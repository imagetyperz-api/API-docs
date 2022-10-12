## How to bypass any captcha with ImageTyperz tasks

The captcha ecosystem has changed dramatically in the last decade, and especially in the last couple of years.

It all started with the classic image captcha, where the user is presented with an image containing characters up to recaptcha, geetest v4, hcaptcha and other complex types.

We decided to release an **entirely new system** with our service, called tasks.
This system will be able to handle all types of captchas, and more than just captchas.

The main concept of the task is the following:

- templates are created by users, on which tasks will operate
- users submit tasks through API, using a template name and variables
- workers load those tasks on their machine and solve the task
- when task is completed, the user will get back the session of the worker

With this the client can literally make his own mini-bot, which will run on worker machines.
When the mini-bot has completed, the user will get the session of the worker, that is: localStorage, cookies and fingerprint.
He can then use that information and restore the session on his end.

<p align="center">
    <h3>Video demonstration</h3>
</p>
<p align="center">
    <a href="https://www.youtube.com/watch?v=fZToUFzeomc"><img src="https://i.imgur.com/kwvF3lY.png"/></a>
</p>


### Templates

An Imagetyperz task template defines the exact steps that the worker should go through. 
Templates consist of actions, which are executed one after the other. When one action is complete, the task moves to the next one. The task will re-run the action until it succeeds. 

Login to [https://imagetyperz.net](https://imagetyperz.net/) to access the templates.

![login](https://i.imgur.com/yUF3hWS.png)

#### What kind of actions are available ?

- **FILL_INPUT_AUTO** - auto complete field value with text                        

- **WAIT_CONTROL_TEXT_PRESENT** - wait for text to appear in dom                        

- **WAIT_CONTROL_TEXT_NOT_PRESENT** - wait for text to disappear from dom                        

- **WAIT_SELECTOR_PRESENT** - wait for CSS selector to appear                        

- **WAIT_SELECTOR_NOT_PRESENT** - wait for CSS selector to disappear                        

- **WAIT_URL_KEYWORD_PRESENT** - wait for keyword (text) in URL to appear                        

- **WAIT_URL_KEYWORD_NOT_PRESENT** - wait for keyword (text) in URL to disappear                        

- **CLICK_ON_SELECTOR** - wait for CSS selector to appear and click on it                        

- **CLICK_ON_ELEMENT_WITH_TEXT** - wait for an element containing specific text to                            appear and click on it                        

- **HIDE_ELEMENT_BY_SELECTOR** - Hide an element by CSS selector to help worker focus                            on task                        

- **CHANGE_DESCRIPTION** - Changes description text for worker. Useful when he's required                            to do another step                        

- **TAKE_SCREENSHOT** - Takes screenshot of current page state                        

- **DELAY_TIME** - Delay for an amount of seconds         

And more will be added.               

Actions can also be set as:

- **optionally** - action can be success or not, task will move to next action on regardless
- **exit Trigger** - can be set for certain actions, with optional flag only. If action succeedsm it will stop the task from execution and return current session to user



You can easily load an example template from our templates website interface.

​											![add template](https://i.imgur.com/H5mqRWp.png)



Each template requires the following:

- **name** - which will be used when submitting tasks with it
- **visibility** - private or public, if private, only you can use it, if public, other users can use and see it too
- **description for customers** - description that will be seen by other customers, when template is set as public
- **description for workers** - what will be seen by the worker when solving it, can also be changed dynamically as task action
- **variables** - information such as email, password, etc, that will be set when submitting a new task or through pushVariables
- **action steps** - sequential steps / actions, that will be executed on the workers machine
- **domains of interest** - other domains for which cookies will be collected (as task solution)

### Publishing templates

You have 2 options when publishing a template: making it either private or public.      

- Private templates are available only with your API key. Other customers can't use them. Cost for reviewing and publishing: $1.
- Public templates are available to everyone. You'll earn %5 on each customer's  expenses with this template. You'll need to leave some contacts for our  customers to reach out for your help if something goes wrong with your  template. Cost for reviewing and publishing: $1.

We review all templates carefully. You need to follow some basic requirements to switch successfully to production mode:      

- No illegal activity of any kind.
- Templates should not duplicate existing ones.
- Don't submit dummy or test templates.
- Provide an example web address and variable values for review (in description). We'll launch a  test, and all the steps should complete successfully.

### Public templates

On https://imagetyperz.net you can see templates that are public and verified already.

You can also search by template name and description.

Templates having the green shield are added by us so they are the most safe to use, from the public templates.

![image-20221011124043346](https://i.imgur.com/XYRoMvw.png)



### Submitting task (API request)

The task information such as template_name, page_url, variables and user-agent are submitted through our API.
Each submission is considered a different run of the template, with the specified information.

```bash
curl -i -s -k -X $'POST' \
    -H $'Content-Type: application/x-www-form-urlencoded' \
    --data-binary $'token=YOUR_ACCESS_TOKEN&action=UPLOADCAPTCHA&pageurl=https://imagetyperz.net/automation/login&variables={"username": "abc", "password": "paZZW0rd"}&template_name=Login test page&captchatype=16' \
http://captchatypers.com/captchaapi/UploadCaptchaTask.ashx


# Response
[{"CaptchaId": "428556458"}]
```

Use the returned captchaID like a regular captcha to get the solution.

To find out all the information regarding the API for submitting tasks, check our [API docs](https://github.com/imagetyperz-api/API-docs#task-bypass-any-captchatype-1)

### Push variables of task

The task allows for variables to be pushed, after the task was submitted.

This is very useful, for example in cases of 2FA.

Here's how to push variables for a certain task:

```bash
curl -i -s -k -X $'POST' \
    -H $'Content-Type: application/x-www-form-urlencoded' \
    --data-binary $'action=GETTEXT&captchaid=YOUR_CAPTCHA_ID&pushVariables=%7B%22twofactor_code%22%3A+%2238493%22%7D&token=YOUR_TOKEN' \
    $'http://captchatypers.com/CaptchaAPI/SaveCaptchaPush.ashx'


# Response
[{"CaptchaId":428622223,"Status":"Push Variables Added"}]
```

Variables that are required by the template, but weren't submitted with the task, will be threated as variables that require push update.

When template reaches action with variable that requires push, it will hold until variable is being pushed.

### Usage of solution (session)

Tasks that are completed successfully will return the following:

- cookies
- localStorage
- fingerprint

Use the cookies, localStorage and fingerprint to restore the session into a different browser.
Technologies such as selenium, puppeteer and playwright allow you to do so.

We've created an application in nodejs using playwright that imports the cookies.
Source code is available here: https://github.com/imagetyperz-api/task-cookies-importer

### Pricing

At this time, we set the price at $2.5 per 1000 tasks. Additionally, every second of the task execution costs 1/60 of the task price. For  example, the task costs $0.0025, and the worker spent 20 seconds solving  it.       
The final cost will be $0.00333 = 0.0025 + (0.0025 / 60 * 20) .    

### Conclusion

The tasks are in *beta* currently.
Feel free to message about your thoughts on tasks.