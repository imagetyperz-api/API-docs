Getting started :books:
---------------

Using our API and our service is easy. We provide **API libraries** for the most popular programming languages currently out there.

On top of this, the source code for them is available on [GitHub](https://github.com/imagetyperz-api)

For those more experienced, that want to build their own library [this](#-endpoints) page is intended to help you in doing so.

We take care of our version control with the help of github. The preferred method to use the libraries is either getting them from their specific package manager such as: bower, nuget, etc or by cloning the repository and executing a ***git pull*** regulary to be up-to-date.

For those not that experienced though, we've provided a download button for each API library, to make it easier.

Libraries :cyclone:
------------
A fast and easy way to integrate our service inside your program

Each library comes with an example
### C-sharp

Library can be installed using [NuGet](https://www.nuget.org/packages/imagetyperz-api-latest/), especially if you're using Visual Studio, this will make things much more easier

The github repository contains a ***binary*** folder as well, which contains the library files already compiled.

Github repository contains a **cli** application as well, which is a ***windows client*** for our service. Can be used easily from command-line  and has all the features that our libraries are having.

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-csharp
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-csharp
)

### Python

Same thing applies to python3. In case you don't have pip already, get it, because that's the easiest to get going, and will help you with next libraries you'll require in the future as well.

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-python3
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-python3
)

### NodeJS

**Javascript** is getting more and more pupularity, especially on the server side. NodeJS is revolutionazing the way websites and web servers are built.

We have a library for nodejs, for running on server side, and a library for javascript, which runs on client side, using jquery.


> Install using npm
```
npm install imagetyperz-api
```

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-nodejs
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-nodejs
)

### JavaScript

Similar to the nodejs library, this library works in a very similar fashion, only difference is that this one is intended to work in browser while the other one on server, with nodejs. 

> Install using npm
```
npm install imagetyperz-api-client
```

> Install using bower
```
bower install imagetyperz-api-client
```

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-javascript
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-javascript
)

### Java

For Java, similar to C#, we have a **cli** application, which is cross-platform, since it's built with Java, runs on everything Java runs.

Another thing to keep in mind is there is a folder ***binary*** which has the library already compiled, as well as the cli application.

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-java/
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-java/
)

### PHP

Although PHP has lost some popularity in the past years, I think it's safe to say that probably more than 50% of the websites out there are still using it as their backend.

We've published the library on both composer aka [packagist](http://packagist.org/) and github

> Install using composer
```
composer require imagetyperzapi/imagetyperzapi
```

> Clone from github
```
git clone git clone https://github.com/imagetyperz-api/imagetyperz-api-php
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-php
)


### Ruby

For ruby, the API library can be installed with [bundle](http://bundler.io/) by modiying the ***Gemfile*** or you can clone it from github and use it directly

> Add this line to Gemfile and run ```bundle install```
```
gem "imagetyperzapi", :git => "git://github.com/imagetyperz-api/imagetyperz-api-ruby.git"
```

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-ruby
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-ruby
)

### UBot

Although not a real programming language, 
UBot might be the choice when it comes to some quick automation

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-ubot
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-ubot
)

Types of captcha :palm_tree:
----
### Image captcha

This is the regular captcha, which we all know, all are familiar with. Those that look like this:

![image captcha](http://i.imgur.com/EAvBjai.png)

This were one of the 1st type of captchas. Their time is almost over, but some websites are still using it and we're still providing solving solution for this as well.

### reCAPTCHA V2 (regular)

This is Google's rcaptcha. It's the 2nd version and it's what most websites are using nowadays. It's the captcha that asks you to pick street signs, cars, and so on. Using the libraries while submiting a recaptcha defaults the completion of recaptcha to this type.

### reCAPTCHA V2 (invisible)

Similar to V2, but different. With this type of reCaptcha, the front-end user gets asked to complete a captcha while form gets submitted, so user `doesn't know` there's a robot verification, until form is submitted.

### reCAPTCHA V3

Latest type of reCaptcha from Google that as of today **22 Aug 2018** is still in beta testing (from what Google advertises)

This reCaptcha somewhat different because it doesn't ask the user anything (for now), but rather Google makes use of the users `experience` with Google services, and returns a token. That token, when verified with the secretkey by the webmaster also returns a score that ranges from `0.1` to `0.9`, `0.9` being the best score and `0.1` the worst.

We're providing solving solutions for this reCaptcha as well, although we are also just like Google into beta testing, as Google goes along too.

### reCAPTCHA Enterprise (v2 & v3)

Enterprise captcha was released back in 2020.
This is targeting bigger companies with lots of traffic. At least for now, in order to use enterprise as a webmaster, Google requires you to apply for it, and puts you through an approval process, before you can create a captcha in their Dev console.

Enterprise captcha is designed to work with all the *non-enteprise* reCAPTCHA types: v2, invisible and v3.
Most likely their plan is to charge the webmasters for usages, while previously it was all *free* (they still train their AI everytime somebody solves it, whether it's free or paid).

Currently, we're supporting enterprise for v2 and v3.

### GeeTest 
Next major captcha that came out after Google's reCAPTCHA. This captcha, asks the user to complete puzzle. When the puzzle is completed, three codes are sent back and needed in order to validate it.

### Capy
Same as Geetest, requires to solve a puzzle. A response is generated, which looks like mouse coordinates of the solving of captcha. The more the mouse/puzzle piece is moved in order to solve the captcha, the bigger the response is.

### hCaptcha
Similar to capy and reCAPTCHA in solving, it requires a pageurl and sitekey in order for it to be solved. It's also the newest one.

### FunCaptcha

Similar to capy

### Tiktok

Captcha from tiktok website is a bit different than the others, but still similar in some regards. Usually it's asking the user to pick certain objects that are alike, from a handful of objects, which look or don't look similar.

### Task (Bypass any captchatype)

The task is a totally different concept compared to the other types of captcha. 
With the other captcha types above, we are instructing our workers to solve that particular captcha and we get a captcha solution back. 
The task is different. You create a template (bot) [here](https://imagetyperz.net) which will contain actions, step by step. Those actions will be executed on the worker computer. If there is a captcha on the page, you can instruct the worker to solve the captcha, and manually click a button, by using the description field of the template. You will get back the cookies, localStorage, fingerprint and screenshot of the worker's browser. This will make it possible for you to restore the session of the worker, i.e automatically logged into an account. Isn't that nice ? :)


Endpoints :sparkles:
--------------
:star2: **UPDATE 2020** :star2:

For getting response of any captcha type submitted, use the JSON response endpoint. 
That's the recommended way of checking for progress and getting solution.

---

If the above libraries do not satisfy your needs, you can build your own library/class, to handle the captcha completion.

The **base** endpoint is `http://www.captchatypers.com`

When you see something like this `/POST /Forms/RequestBalanceToken.ashx` it's actually 

```
/POST http://www.captchatypers.com/Forms/RequestBalanceToken.ashx
```

### :satellite: Authentication
In order to use our service, one has to make a  **HTTP POST** request to our server, which will respond accordingly, depending on what was requested.

Each request you make, needs to contain authentication data, in order for our server to verify it's identity and integrity.

Initially, our API service was designed to work with **username & password** for authentication.

We've updated our system, to work with **access tokens** as well, which is much more safe and convenient. One reason is the password of your account is not sent through the wires anymore. Another reason, in case you gave the access token to somebody and want to revoke access, you can easily renew your token, from the [dashboard](https://www.imagetyperz.com/Forms/NewClientHome.aspx) without changing your account's password, etc.


Our system currently **accepts both authentication methods**, with username & password and with access token.

For **username & password**, there is a set of endpoints/urls, and for the **access token** authentication there's another set.

Below, you'll find the methods our API service accepts such as submiting regular captcha, getting account's balance, etc.

**The domain for which the requests are being made is captchatypers.com**


Inside each method, you'll find both types of authentication, with access token and with username & password.

**OBS** Although our system accepts both methods currently, the **access token** method is **preferred** and the username & password authorization method might be removed in the future.

**Responses**

The server will respond with the data that was requested.

The responses are in plain text. 

In case of error, the response text will start with ```ERROR: ```

### :dollar: Balance​

In order to get the balance of your account, the balance endpoints are used.

To get the balance we make a POST request, eg ```http://captchatypers.com/Forms/RequestBalanceToken.ashx```
This would be the URL using access token authentication.

The balance endpoint is one of the easiest to use. It works by making the request, either with token or username & password, and the action parameter. 

> Access token authentication

>```/POST /Forms/RequestBalanceToken.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - action = REQUESTBALANCE
> -------
> Username & password authentication

>```/POST /Forms/RequestBalanceToken.ashx```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - action = REQUESTBALANCE

**Response**

In case of **success**, server will respond with the accounts current balance in USD.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_REQUEST``` - It will be returned when the program tries to send the invalid  request.

- ```ERROR: INVALID_USERNAME``` - If the username is not provided, this will be returned.

- ```ERROR: INVALID_PASSWORD``` - if the password is not provide, this will be returned.

## Image captcha (classic)

Use this enpoint if you want to solve a image captcha. That is, an image with captcha text in it. 

This is also what's called ***classic captcha***, because it's the first one that came into being, way before recaptcha. Some websites are still using it today though.

In order to use this endpoint, the image file has to be sent encoded as a base64 string.

If you authenticate with access token, you can send a HTTP URL instead of the base64 string. The request has to be made to a different endpoint though.

### Observation

**Solving this type of captcha through service is somewhat different compared to all the other types.
When it's submitted, the request will *hold* until the worker solves the captcha, after which the response will be generated for that request. The response will contain both the captcha ID and text (solution for captcha). All the other captcha types work a bit differently. With the other captchas, you submit the captcha, get back an ID right on the spot, and using that ID you regularly check for solution.**


> Access token authentication (base 64)

>```/POST /Forms/UploadFileAndGetTextNEWToken.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - file = ***image file encoded as base64 string***
>
> - action = UPLOADCAPTCHA
>
> - iscase = `true`, if image captcha text is case-sensitive `- optional`
>
> - isphrase = `true`, text contains at least one space `- optional`
>
> - ismath = `true`, instructs worker that a math captcha has to be calculated `- optional`
>
> - alphanumeric = `1`, captcha text contains digits only or `2` if it contains letters only `- optional`
>
> - minlength = `number` - minimum text length, `0` is default, if defined, give bigger or equal to `1` `- optional`
>
> - maxlength = `number` - maximum text length, `0` is default (disabled), if defined it should be bigger than `minlength` `- optional`
>
> - affiliateid = ***affiliateID*** `- optional`
> -------
> Access token authentication (HTTP URL)
> 
>```/POST /Forms/FileUploadAndGetTextCaptchaURLToken.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - file = ***http image url, eg. ```http://abc.com/image.jpg```***
>
> - action = UPLOADCAPTCHA
>
> - iscase = `true`, if image captcha text is case-sensitive `- optional`
>
> - isphrase = `true`, text contains at least one space `- optional`
>
> - ismath = `true`, instructs worker that a math captcha has to be calculated `- optional`
>
> - alphanumeric = `1`, captcha text contains digits only or `2` if it contains letters only `- optional`
>
> - minlength = `number` - minimum text length, `0` is default, if defined, give bigger or equal to `1` `- optional`
>
> - maxlength = `number` - maximum text length, `0` is default (disabled), if defined it should be bigger than `minlength` `- optional`
>
> - affiliateid = ***affiliateID*** `- optional`
> -------
> Username & password authentication

>```/POST /Forms/UploadFileAndGetTextNEW.ashx```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - file = ***image file encoded as base64 string***
>
> - action = UPLOADCAPTCHA
>
> - chkCase = ***1 in case it's sensitive*** ```- optional```
>
> - affiliateid = ***affiliateID*** ```- optional```


**Response**

When request is **successful** the response body will contain both a captcha ID and the text recognized.

Eg.  ```123|polum```

- 123 - the captcha ID
- polum - the recognized text

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_REQUEST``` - It will be returned when the program tries to send the invalid request.

- ```ERROR: INVALID_USERNAME``` - If the username is not provided, this will be returned.

- ```ERROR: INVALID_PASSWORD``` - if the password is not provide, this will be returned.

- ```ERROR: INVALID_AFFILIATEID``` - If the affiliateid is not provided, this will be returned.

- ```ERROR: INVALID_IMAGE_FILE``` - No file uploaded or No image type file uppassword = your password (optional, use only if token is missing)loaded.

- ```ERROR: INVALID_IMAGE_SIZE_30_KB``` - The uploading image file must be 30 KB.

- ```ERROR: NOT_DECODED``` - This is not really an error, just informs the captcha is still under completion. When you get this, ***retry*** after 5 seconds

- ```ERROR: IMAGE_TIMED_OUT``` - Happens when captcha timed out. In other words, it wasn't completed by our workers in time


## reCAPTCHA

### Submit reCAPTCHA

In order to solve regular (v2), invisible or v3 reCAPTCHA, there are **2 steps** that have to be made.

First is to submit the recaptcha details, and then get the **g-response** after it was completed.

This endpoints are used to submit the captcha details, such as pageurl and sitekey, along with the authentication. Check the retrieve recaptcha [page](#-endpoints-retrieve-recaptcha-response) for how to get the response after submission.

There are few optional parameters as well.


> Access token authentication

>```/POST /captchaapi/UploadRecaptchaToken.ashx```

> **Parameters**
>
> - token = ***your_access_token***
> - pageurl = ***page url of website, eg. ```abc.com```***
> - googlekey = ***sitekey of recaptcha, has to be scraped from site***
> - action = UPLOADCAPTCHA
> - recaptchatype = can be one of this 3 values: `1` - normal, `2` - invisible, `3` - v3 (it's optional, defaults to `1`)
> - captchaaction = action parameter used in solving v3 recaptcha `- optional`
> - domain = used in loading reCAPTCHA interface, default: www.google.com (alternative: recaptcha.net) `- optional`
> - score = score targeted, check being done against a test recaptcha `- optional`
> - affiliateid = ***affiliateID*** ```- optional```
> - proxy = ***if given, captcha will be solved using proxy, eg. ```12.34.56.78:1234``` also works with private proxies (auth) like this: ```12.34.56.78:1234:username:password```*** ```- optional```
> - proxytype = ```HTTP```, in case proxy parameter is set. Currently, only HTTP proxies are supported. ```- optional```
> - useragent = User-Agent used in solving recaptcha `- optional`
> - data-s = required with some recaptchas. A one-time token generated with each captcha loaded `- optional`
> - cookie_input = cookies used in solving reCAPTCHA `- optional`
>
> Username & password authentication

>```/POST /captchaapi/UploadRecaptchaV1.ashx```

> **Parameters**
>
> - username = ***your_username***
> - password = ***your_password***
> - pageurl = ***page url of website, eg. ```abc.com```***
> - googlekey = ***sitekey of recaptcha, has to be scraped from site***
> - action = UPLOADCAPTCHA
> - recaptchatype = can be one of this 3 values: `1` - normal, `2` - invisible, `3` - v3 (it's optional, defaults to `1`)
> - captchaaction = action parameter used in solving v3 recaptcha `- optional`
> - domain = used in loading reCAPTCHA interface, default: www.google.com (alternative: recaptcha.net) `- optional`
> - score = score targeted, check being done against a test recaptcha `- optional`
> - affiliateid = ***affiliateID*** ```- optional```
> - proxy = ***if given, captcha will be solved using proxy, eg. ```12.34.56.78:1234``` also works with private proxies (auth) like this: ```12.34.56.78:1234:username:password```*** ```- optional```
> - proxytype = ```HTTP```, in case proxy parameter is set. Currently, only HTTP proxies are supported. `- optional`
> - useragent = User-Agent used in solving recaptcha `- optional`
> - data-s = required with some recaptchas. A one-time token generated with each captcha loaded `- optional`
> - cookie_input = cookies used in solving reCAPTCHA `- optional`
### Submit reCAPTCHA enterprise (2021 update)

Submission is very similar to non-enterprise reCAPTCHA types.


> Access token (or user / password) authentication

>```/POST /captchaapi/UploadRecaptchaEnt.ashx```

> **Parameters**
>
> - token = ***your_access_token***
> - username = ***your_username*** (deprecated, token authentication is preferred)
> - password = ***your_password***
> - pageurl = ***page url of website, eg. ```abc.com```***
> - googlekey = ***sitekey of recaptcha, has to be scraped from site***
> - action = UPLOADCAPTCHA
> - enterprise_type = v2 or v3 `- optional, defaults to v2`
> - captchaaction = action parameter used in solving of v3 type `- optional`
> - domain = used in loading reCAPTCHA interface, default: www.google.com (alternative: recaptcha.net) `- optional`
> - score = score targeted, check being done against a test recaptcha `- optional`
> - affiliateid = ***affiliateID*** ```- optional```
> - proxy = ***if given, captcha will be solved using proxy, eg. ```12.34.56.78:1234``` also works with private proxies (auth) like this: ```12.34.56.78:1234:username:password```*** ```- optional```
> - proxytype = ```HTTP```, in case proxy parameter is set. Currently, only HTTP proxies are supported. ```- optional```
> - useragent = User-Agent used in solving recaptcha `- optional`
> - data-s = required with some recaptchas. A one-time token generated with each captcha loaded `- optional`
> - cookie_input = cookies used in solving reCAPTCHA `- optional`

**Response**

As a response, you'll get back a ```captchaID``` number in case of success.

This ```captchaID``` will be used in the 2nd step, to retrieve the g-response after our workers have completed the captcha.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_DOMAIN``` - Wrong domain. Check your domain.

- ```ERROR: INVALID_SITEKEY```- Wrong site key. Check your site key.

- ```ERROR: AUTOMATED_QUERIES``` - Proxy sent is blocked temporarily. Change your proxy.

- ```ERROR: NOT_INVISIBLE``` - Captcha is not invisible

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

### Retrieve reCAPTCHA response (deprecated)

**Deprecated**

*Use JSON response endpoint*

---

Once you have the ```captchaID```, you can start checking for the g-response.

Usually, it takes ~20-50 seconds for our workers to complete the captcha.

The idea is to check regulary if the ID was completed. It's safe to check every 5 seconds for the g-response, in other words make the request every 5 seconds.

To get a better picture, check our libraries, even if you want to build your own library, would be helpful to see how a library and the example file that comes with it were built.

> Access token authentication

>```/POST /captchaapi/GetRecaptchaTextToken.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - captchaID = ***```captchaID``` gathered before***
>
> - action = GETTEXT
> -------
> Username & password authentication

>```/POST /captchaapi/GetRecaptchaText.ashx```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - captchaID = ***```captchaID``` gathered before***
>
> - action = GETTEXT

**Responses**

When our workers have completed the captcha, you will get back a g-response, which in turn, can be used to bypass the captcha on the website. 

The g-response looks like this: ```03ANcjosrFMmAAFkgiX1...kuZmKh5v0```

[Here](https://www.imagetyperz.com/Forms/recaptcha_automation.aspx) are few examples on how to use the g-response in a ***real-life situation***

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_DOMAIN``` - Wrong domain. Check your domain.

- ```ERROR: INVALID_SITEKEY```- Wrong site key. Check your site key.

- ```ERROR: AUTOMATED_QUERIES``` - Proxy sent is blocked temporarily. Change your proxy.

- ```ERROR: NOT_INVISIBLE``` - Captcha is not invisible

- ```ERROR: NOT_DECODED``` - This is not really an error, just informs the captcha is still under completion. When you get this, ***retry*** after 5 seconds

- ```ERROR: IMAGE_TIMED_OUT``` - Happens when captcha timed out. In other words, it wasn't completed by our workers in time

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## GeeTest

### Submit GeeTest

GeeTest is another captcha that our service can handle.

Similar to reCAPTCHA, geetest captcha details are submitted, ID is received and using that ID periodically to check for completion.
> Access token authentication

>```GET /captchaapi/UploadGeeTestToken.ashx?action=UPLOADCAPTCHA&domain=geetest_domain&challenge=geetest_challenge&gt=geetest_gt&username=your_username&password=your_password&affiliateid=your_affiliate_id[optional]```

> **Parameters**
>
> - token = ***your access token***
>
> - domain = ***geetest captcha domain***
>
> - challenge = ***geetest captcha challenge key***
>
> - gt = ***geetest captcha gt key***
>
> - api_server = ***geetest API domain*** ```- optional```
>
> - action = UPLOADCAPTCHA
>
> - affiliateid = ***affiliateID*** ```- optional```
>
> - useragent = ***user agent goes here*** ```- optional```
>
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> -------
> Username & password authentication

>```GET /captchaapi/UploadGeeTest.ashx?action=UPLOADCAPTCHA&domain=geetest_domain&challenge=geetest_challenge&gt=geetest_gt&username=your_username&password=your_password&affiliateid=your_affiliate_id[optional]```

> **Parameters**
>
> - username = ***your username***
>
> - password = ***your password***
>
> - domain = ***geetest captcha domain***
>
> - challenge = ***geetest captcha challenge key***
>
> - gt = ***geetest captcha gt key***
>
> - api_server = ***geetest API domain*** ```- optional```
>
> - action = UPLOADCAPTCHA
>
> - affiliateid = ***affiliateID*** ```- optional```
>
> - useragent = ***user agent goes here*** ```- optional```
>
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```

**Response**

`captchaID` is returned back. Use that to retrieve the 3 geetest keys, once completed.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.
- ```ERROR: INVALID_GEETEST_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load geetest captcha on worker end
- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

### Submit GeeTestV4

GeeTesV4 is a new version of captcha from geetest

> Access token (or username & password) authentication

>```POST /captchaapi/UploadGeeTestV4.ashx```

> **Parameters**
>
> - token = ***your access token*** (preferred method to authenticate, use username & password only when really necessary)
> - username = account username `- optional` 
> - password = account password `- optional` 
> - domain = ***geetest captcha domain***
> - geetestid = ***geetest captcha ID***
> - action = UPLOADCAPTCHA
> - affiliateid = ***affiliateID*** ```- optional```
> - useragent = ***user agent goes here*** ```- optional```
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```

### Retrieve GeeTest response (deprecated)

Once you have the ```captchaID```, you can start checking for the g-response.

Usually, it takes ~10 seconds for our workers to complete the captcha.

The idea is to check regulary if the ID was completed. It's safe to check every 5 seconds for the response, in other words make the request every 5 seconds.

> Access token authentication

>```GET /captchaapi/getrecaptchatext.ashx?token=your_access_token&captchaID=your_captcha_ID&action=GETTEXT```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - captchaID = ***```captchaID``` gathered before***
>
> - action = GETTEXT
> -------
> Username & password authentication

>```GET /captchaapi/getrecaptchatext.ashx?username=your_username&password=your_password&captchaID=your_captcha_ID&action=GETTEXT```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - captchaID = ***```captchaID``` gathered before***
>
> - action = GETTEXT


**Responses**

Once the geetest captcha was successfully completed by our workers you will get 3 codes back.

They're formatted like this in the response: ***challenge;;;validate;;;seccode*** 

ie. `a70928569b0666a987bec2c0003ac2cfb4;;;32d47af0b8cf8c029ba698cb074ceecd;;;32d47af0b8cf8c029ba698cb074ceecd|jordan`

Use the 3 codes to bypass the geetest captcha.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.
- ```ERROR: INVALID_GEETEST_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load geetest captcha on worker end
- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## Capy

> Access token authentication (or user & password)

>```POST /captchaapi/UploadCapyCaptchaUser.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - captchatype = **12**
> - pageurl = **the URL where you got the captcha**
> - sitekey = **sitekey used in solving captcha (gathered from URL source code / DOM)**
> - action = **UPLOADCAPTCHA**
> - affiliateid = ***affiliateID*** ```- optional```
> - useragent = ***user agent goes here*** ```- optional```
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> 

**Response**

`captchaID` is returned back, use it with response JSON endpoint to retrieve solution.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load capy captcha on worker end

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## hCaptcha

> Access token authentication (or user & password)

>```POST /captchaapi/UploadHCaptchaUser.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - captchatype = **11**
> - pageurl = **the URL where you got the captcha**
> - sitekey = **sitekey used in solving captcha (gathered from URL source code / DOM)**
> - action = **UPLOADCAPTCHA**
> - affiliateid = ***affiliateID*** ```- optional```
> - apiEndpoint = domain used in loading of hcaptcha interface, default: `hcaptcha.com` - `optional`
> - useragent = ***user agent goes here*** ```- optional```
> - invisible = **1, if hcaptcha is invisible** ```- optional```
> - HcaptchaEnterprise = **extra payload used in loading hcaptcha, e.g rqdata, JSON stringified format** `- optional`
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> 

**Response**

`captchaID` is returned back, use it with response JSON endpoint to retrieve solution.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load hcaptcha on worker end

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## Tiktok

> Access token authentication (or user & password)

>```POST /captchaapi/UploadTikTokCaptchaUser.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - captchatype = **10**
> - pageurl = **the URL where you got the captcha**
> - cookie_input = **cookies that will be set when solving captcha**
> - action = **UPLOADCAPTCHA**
> - affiliateid = ***affiliateID*** ```- optional```
> - useragent = ***user agent goes here*** ```- optional```
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> 

**Response**

`captchaID` is returned back, use it with response JSON endpoint to retrieve solution.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load tiktok captcha on worker end

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## FunCaptcha (Arkose Labs)

> Access token authentication (or user & password)

>```POST /captchaapi/UploadFunCaptcha.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - captchatype = **13**
> - pageurl = **the URL where you got the captcha**
> - sitekey = **sitekey/publickey used in solving captcha (gathered from URL source code / DOM)**
> - s_url = **API / source URL, specific for FunCaptcha**
> - action = **UPLOADCAPTCHA**
> - data = **extra parameters in JSON format, used when initializing captcha** `- optional`
> - affiliateid = ***affiliateID*** ```- optional```
> - useragent = ***user agent goes here*** ```- optional```
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> 

**Response**

`captchaID` is returned back, use it with response JSON endpoint to retrieve solution.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.
- ```ERROR: INVALID_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load funcaptcha captcha on worker end
- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## Turnstile (Cloudflare)

> Access token authentication (or user & password)

>```POST /captchaapi/Uploadturnstile.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - pageurl = **the URL where you got the captcha**
> - sitekey = **sitekey used in solving captcha (gathered from URL source code / DOM)**
> - action = **UPLOADCAPTCHA**
> - affiliateid = ***affiliateID*** ```- optional```
> - domain = domain used in loading turnstile interface, default: `challenges.cloudflare.com` - `optional`
> - taction = used in loading turnstile interface, similar to reCAPTCHA `- optional`
> - data = extra parameter used in loading turnstile interface `- optional`
> - useragent = user agent used in solving the captcha ```- optional```
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> 

**Response**

`captchaID` is returned back, use it with response JSON endpoint to retrieve solution.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

- ```ERROR: INVALID_CAPTCHA_DATA``` - Keys expired or other reason for not being able to load capy captcha on worker end

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

## Task (Bypass any captchatype)

> Access token authentication (or user & password)

>```POST /captchaapi/UploadCaptchaTask.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - captchatype = **16**
> - template_name = **name of the template that will be executed**
> - pageurl = **the URL on which the template will be executed**
> - variables = **variables that are used in the template execution, in stringified JSON format**
> - action = **UPLOADCAPTCHA**
> - affiliateid = ***affiliateID*** ```- optional```
> - useragent = ***user agent goes here*** ```- optional```
> - proxy = ***eg. 123.45.67.89:1234 or 12.34.56.78:123:username:password*** ```- optional```
>
> 

**Response**

`captchaID` is returned back, use it with response JSON endpoint to retrieve solution.

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.
- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

### Push variables for task
Update a variable value **while task is running on worker machine**. Useful when dealing with 2FA authentication.

When template reaches an action that uses a variable which wasn't provided with the submission of the task,
task (while running on worker machine) will wait for variable to be updated through push.

You can use the pushVariables method as many times as you need, even overwriting previously set variables.

> Access token authentication (or user & password)

>```POST /captchaapi/UploadCaptchaTask.ashx```

> **Parameters**
>
> - token = ***your access token***
> - username = ***your username*** (token is preferred)
> - password = **your password** (token is preferred)
> - captchaid = **ID of task captcha**
> - pushVariables = **push variables that are used in the template execution, in stringified JSON format**
> - action = **GETTEXT**
> 

**Response**

`[{"CaptchaId":123456,"Status":"Push Variables Added"}]`

**Errors**

- ```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access key are invalid.

## Response JSON endpoint

This is the recommended way of getting the response for any captcha type in JSON format, once ID of captcha was received from submission.

> Access token authentication (or username & password, deprecated)

>```GET /captchaapi/GetCaptchaResponseJson.ashx ```

> **Parameters**
>
> - token = ***your_access_token***
> - username=**your_username** (token is preferred)
> - password=**your_password** (token is preferred)
> - captchaid = ***```captchaID``` gathered before***
> - action = GETTEXT

Response looks like this

```json
{
  "CaptchaId": 176707908, 
  "Response": "03AGdBq24PBCbwiDRaS_MJ7Z...mYXMPiDwWUyEOsYpo97CZ3tVmWzrB", 
  "Cookie_OutPut": "", 
  "Proxy_reason": "", 
  "Recaptcha score": 0.0, 
  "Status": "Solved"
}
```

## Other

### Set captcha bad

If the response you've received from our server was for some reason wrong, you can notify us by making a request to this endpoint/s.

The ```captchaID``` that was wrong has to be sent along with the authentication and action parameter set to ```SETBADIMAGE```

> Access token authentication

>```/POST /Forms/SetBadImageToken.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - imageid = ***```captchaID``` that was solved wrong***
>
> - action = SETBADIMAGE
> -------
> Username & password authentication

>```/POST /Forms/SetBadImage.ashx```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - imageid = ***```captchaID``` that was solved wrong***
>
> - action = SETBADIMAGE

**Responses**

In case of success, server will respond with ```SUCCESS```

### Was proxy used (deprecated)

A way to check if proxy submitted with captcha was used in solving

Can be used only after captcha is completed, and can be also used to get gresponse
> Access token authentication

>```/POST /captchaAPI/GetReCaptchaTextJSON.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - captchaid = ***```captchaID``` - captcha id that you want to check proxy for***
>
> - action = GETTEXT
> -------
> Username & password authentication

>```/POST /captchaAPI/GetReCaptchaTextTokenJSON.ashx```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - captchaid = ***```captchaID``` - captcha id that you want to check proxy for***
>
> - action = GETTEXT

**Responses**

```json
{	"Proxy_worker":"12.34.56.78:4321",
	"Result":"03AE...gMofH2rqQ6bFG",
	"Proxy_client":"12.34.56.78:4321",
	"Proxy_reason":""
}
```

If you submitted a proxy and it wasn't used, `Proxy_reason` will contain the error of why the proxy wasn't used.

`Proxy_worker` contains proxy used by worker. `Proxy_client` being the proxy value submitted with the captcha. 

When proxy was successfully used they should both contain the same value.


### Errors

-```ERROR: AUTHENTICATION_FAILED``` - Provided username and password and/or access token are invalid.

-```ERROR: INVALID_REQUEST``` - It will be returned when the program tries to send the invalid request.

-```ERROR: INVALID_USERNAME``` - If the username is not provided, this will be returned.

-```ERROR: INVALID_PASSWORD``` - if the password is not provide, this will be returned.

-```ERROR: INVALID_IMAGE_ID``` - Not provided image id or Provided invalid image id.


Proxies
----------
In case you're submitting the reCaptchas with proxies, check for gresponse validity. In case gresponse token is not valid, change the proxy because
it might be banned by Google.

You can also check if proxy was used or not by using the [was proxy used](#was-proxy-used) methods available in our API libraries and API.


Automation examples
------------------------------
We've made automation examples for both normal and invisible recaptcha, with and without browser. The examples can be found [here](https://www.imagetyperz.com/Forms/recaptcha_automation.aspx)


2captcha,DBC and anticaptcha api support
--------------------

We've designed a captcha gate, which allows you to redirect traffic from other captcha services through imagetyperz. Currently, we've integrated the following services:
- 2captcha.com
- deathbycaptcha.com
- anti-captcha.com

### Redirection
The gates are redirecting the following actions to our service:

- get balance
- submit image captcha
- retrieve image captcha
- submit recaptcha
- retrieve recaptcha response


In other words, if you have software that works with any of the above services, using the gate will allow you to **use our service, with the same software**.

This is achieved by running a **batch** program, that writes config information into the ***hosts*** file of the Windows operating system. All this is done automatically, all you have to do is run it. For linux, we have a python script that allows you to toggle (enable / disable) a pair of **IP    DOMAIN** 

The last step, is to use **replace access token OR username & password with credentials from magetyperz**. In this way, the programs will run even though they were built for one of the services above, but in reality our service will be used for completion.

In case you don't want to use the gate anymore, you can edit the hosts file which is located here: `%SystemRoot%\System32\drivers\etc\hosts`

On linux, you'll find the hosts file in `/etc/hosts`

Both operating systems require admin / root access in order to modify the files

For more details about the hosts file check [this](https://www.howtogeek.com/howto/27350/beginner-geek-how-to-edit-your-hosts-file/) link


> **Installation**

> Clone the github repository
```
git clone https://github.com/imagetyperz-api/gates
```

Once you got it, go to ***scripts/windows*** folder, and run bat file for the service you want to redirect

It will ask you for administrator rights, because it's writing to a system file, allow it, and the gate should be enabled within few seconds

For linux, here's the usage of the script: `./linux_hosts.py 127.0.0.1 site.com` which can be found in ***scripts/linux***

> [View on github >]( https://github.com/imagetyperz-api/gates
)
