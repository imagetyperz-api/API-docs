Getting started
---------------

Using our API and our service is easy. We provide **API libraries** for the most popular programming languages currently out there.

On top of this, the source code for them is available on [github](https://github.com/imagetyperz-api), and most of them are available on their own package managers such as:

* npm
* nuget
* pypi
* bower
* composer

For those more experienced, that want to build their own library [this](#-endpoints) page is intended to help you in doing so.

We take care of our version control with the help of github. The preferred method to use the libraries is either getting them from their specific package manager such as: bower, nuget, etc or by cloning the repository and executing a ***git pull*** regulary to be up-to-date.

For those not that experienced though, we've provided a download button for each API library, to make it easier.

Libraries
------------
A fast and easy way to integrate our service inside your program

Each library comes with an example
### C-sharp

Library can be installed using [NuGet](https://www.nuget.org/packages/imagetyperz-api-latest/), especially if you're using Visual Studio, this will make things much more easier

The github repository contains a ***binary*** folder as well, which contains the library files already compiled.

Github repository contains a **cli** application as well, which is a ***windows client*** for our service. Can be used easily from command-line  and has all the features that our libraries are having.

> Install using nuget
```
Install-Package imagetyperz-api-latest
```

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-csharp
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-csharp
)

> [Download >](https://github.com/imagetyperz-api/imagetyperz-api-csharp/archive/master.zip)

### Python 2.x
This is how you can get the library for python version 2. We have it for python3 as well, below.

**pip** is a popular package manager for python, which usually comes installed with the OS python installation, in case of linux.

If you're on windows and not linux or mac, first, **make sure you have python2 installed**, and grab download pip installation file from [here](https://bootstrap.pypa.io/get-pip.py)

All you have to do is open the file and pip will get installed. 

Once that's done, you can find pip inside the ***Scripts*** folder, of the python installation.

> Install using pip
```
pip2 install imagetyperzapi2
```

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-python2
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-python2
)

> [Download >](https://github.com/imagetyperz-api/imagetyperz-api-python2/archive/master.zip)

### Python 3.x

Same thing applies to python3. In case you don't have pip already, get it, because that's the easiest to get going, and will help you with next libraries you'll require in the future as well.

> Install using pip
```
pip3 install imagetyperzapi3
```

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-python3
```

> [View on github >](https://github.com/imagetyperz-api/imagetyperz-api-python3
)

> [Download >](https://github.com/imagetyperz-api/imagetyperz-api-python3/archive/master.zip)


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

> [Download >](https://github.com/imagetyperz-api/imagetyperz-api-nodejs/archive/master.zip)


### Javascript

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

> [Download >](https://github.com/imagetyperz-api/imagetyperz-api-javascript/archive/master.zip)

### Java

For Java, similar to C#, we have a **cli** application, which is cross-platform, since it's built with Java, runs on everything Java runs.

Another thing to keep in mind is there is a folder ***binary*** which has the library already compiled, as well as the cli application.

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-java/
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-java/
)

> [Download >]( https://github.com/imagetyperz-api/imagetyperz-api-java//archive/master.zip)

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

> [Download >]( https://github.com/imagetyperz-api/imagetyperz-api-php/archive/master.zip)


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

> [Download >]( https://github.com/imagetyperz-api/imagetyperz-api-ruby/archive/master.zip)

### Perl

We have a library for the ***good-ol'-perl*** as well

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-perl
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-perl
)

> [Download >]( https://github.com/imagetyperz-api/imagetyperz-api-perl/archive/master.zip)

### UBot

Although not a real programming language, 
UBot might be the choice when it comes to some quick automation

> Clone from github
```
git clone https://github.com/imagetyperz-api/imagetyperz-api-ubot
```

> [View on github >]( https://github.com/imagetyperz-api/imagetyperz-api-ubot
)

> [Download >]( https://github.com/imagetyperz-api/imagetyperz-api-ubot/archive/master.zip)

Types of captcha
----
### Image captcha

This is the regular captcha, which we all know, all are familiar with. Those that look like this:

![image captcha](http://i.imgur.com/EAvBjai.png)

This were one of the 1st type of captchas. Their time is almost over, but some websites are still using it and we're still providing solving solution for this as well.

### reCaptcha V2 (regular)

This is Google's rcaptcha. It's the 2nd version and it's what most websites are using nowadays. It's the captcha that asks you to pick street signs, cars, and so on. Using the libraries while submiting a recaptcha defaults the completion of recaptcha to this type.

### reCaptcha V2 (invisible)

Similar to V2, but different. With this type of reCaptcha, the front-end user gets asked to complete a captcha while form gets submitted, so user `doesn't know` there's a robot verification, until form is submitted.

### reCaptcha V3 (NEW)

Latest type of reCaptcha from Google that as of today **22 Aug 2018** is still in beta testing (from what Google advertises)

This reCaptcha somewhat different because it doesn't ask the user anything (for now), but rather Google makes use of the users `experience` with Google services, and returns a token. That token, when verified with the secretkey by the webmaster also returns a score that ranges from `0.1` to `0.9`, `0.9` being the best score and `0.1` the worst.

We're providing solving solutions for this reCaptcha as well, although we are also just like Google into beta testing, as Google goes along too.

Endpoints
--------------
If the above libraries do not satisfy your needs, you can build your own library/class, to handle the captcha completion.

The **base** endpoint is `http://www.captchatypers.com`

When you see something like this `/POST /Forms/RequestBalanceToken.ashx` it's actually 

```
/POST http://www.captchatypers.com/Forms/RequestBalanceToken.ashx
```

### Authentication
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

### Balance

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

### Image captcha (classic)

Use this enpoint if you want to solve a image captcha. That is, an image with captcha text in it. 

This is also what's called ***classic captcha***, because it's the first one that came into being, way before recaptcha. Some websites are still using it today though.

In order to use this endpoint, the image file has to be sent encoded as a base64 string.

If you authenticate with access token, you can send a HTTP URL instead of the base64 string. The request has to be made to a different endpoint though.

The parameter ```chkCase``` in the requests, if set to 1, will tell our workers that the captcha is case sensitive, and it has to be completed so.


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
> - chkCase = ***1 in case it's sensitive*** ```- optional```
>
> - affiliateid = ***affiliateID*** ```- optional```
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
> - chkCase = ***1 in case it's sensitive*** ```- optional```
>
> - affiliateid = ***affiliateID*** ```- optional```
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

- ```ERROR: INVALID_IMAGE_FILE``` - No file uploaded or No image type file uploaded.

- ```ERROR: INVALID_IMAGE_SIZE_30_KB``` - The uploading image file must be 30 KB.

- ```ERROR: NOT_DECODED``` - The captcha has timedout


### Submit reCaptcha

In order to solve recaptcha v2 and invisible, there are **2 steps** that have to be made.

First is to submit the recaptcha details, and then get the **g-response** after it was completed.

This endpoints are used to submit the captcha details, such as pageurl and sitekey, along with the authentication. Check the retrieve recaptcha [page](#-endpoints-retrieve-recaptcha-response) for how to get the response after submission.

There are few optional parameters as well.


> Access token authentication

>```/POST /captchaapi/UploadRecaptchaToken.ashx```

> **Parameters**
> 
> - token = ***your_access_token***
>
> - pageurl = ***page url of website, eg. ```abc.com```***
>
> - googlekey = ***sitekey of recaptcha, has to be scraped from site***
>
> - action = UPLOADCAPTCHA
>
> - recaptchatype = can be one of this 3 values: `1` - normal, `2` - invisible, `3` - v3 (it's optional, defaults to `1`)
>
> - captchaaction = action parameter used in solving v3 recaptcha `- optional`
>
> - score = score targeted, check being done against a test recaptcha `- optional`
>
> - affiliateid = ***affiliateID*** ```- optional```
>
> - proxy = ***if given, captcha will be solved using proxy, eg. ```12.34.56.78:1234``` also works with private proxies (auth) like this: ```12.34.56.78:1234:username:password```*** ```- optional```
>
>- useragent = User-Agent used in solving recaptcha `- optional`
>
> - proxytype = ```HTTP```, in case proxy parameter is set. Currently, only HTTP proxies are supported. ```- optional```
> -------
> Username & password authentication

>```/POST /captchaapi/UploadRecaptchaV1.ashx```

> **Parameters**
> 
> - username = ***your_username***
>
> - password = ***your_password***
>
> - pageurl = ***page url of website, eg. ```abc.com```***
>
> - googlekey = ***sitekey of recaptcha, has to be scraped from site***
>
> - action = UPLOADCAPTCHA
>
> - recaptchatype = can be one of this 3 values: `1` - normal, `2` - invisible, `3` - v3 (it's optional, defaults to `1`)
>
> - captchaaction = action parameter used in solving v3 recaptcha `- optional`
>
> - score = score targeted, check being done against a test recaptcha `- optional`
>
> - affiliateid = ***affiliateID*** ```- optional```
>
> - proxy = ***if given, captcha will be solved using proxy, eg. ```12.34.56.78:1234``` also works with private proxies (auth) like this: ```12.34.56.78:1234:username:password```*** ```- optional```
>
>- useragent = User-Agent used in solving recaptcha `- optional`
>
> - proxytype = ```HTTP```, in case proxy parameter is set. Currently, only HTTP proxies are supported. ```- optional```

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

### Retrieve reCaptcha response

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

- ```ERROR: NOT_DECODED``` - This is a ***positive*** error, which informs the captcha is still under completion. When you get this, ***retry*** after 5 seconds

- ```ERROR: INVALID_DOMAIN``` - Wrong domain. Check your domain.

- ```ERROR: INVALID_SITEKEY```- Wrong site key. Check your site key.

- ```ERROR: AUTOMATED_QUERIES``` - Proxy sent is blocked temporarily. Change your proxy.

- ```ERROR: NOT_INVISIBLE``` - Captcha is not invisible

- ```ERROR: LIMIT_EXCEED``` - Server is overloaded

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

### Was proxy used

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

> [Download >]( https://github.com/imagetyperz-api/gates/archive/master.zip)
