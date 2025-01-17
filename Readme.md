Angular Socialshare
==================

![Angular socialshare](http://i.imgur.com/sqnePat.png)

[![Join the chat at https://gitter.im/720kb/angular-socialshare](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/720kb/angular-socialshare?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


Angular Socialshare is an angularjs directive for sharing urls and content on social networks such as (facebook, google+, twitter, pinterest and so on).


The Angular Socialshare is developed by [720kb](http://720kb.net).

####Requirements


AngularJS v1.3+

####Browser support


![Chrome](https://raw.github.com/alrra/browser-logos/master/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/alrra/browser-logos/master/firefox/firefox_48x48.png) | ![IE](https://raw.github.com/alrra/browser-logos/master/internet-explorer/internet-explorer_48x48.png) | ![Opera](https://raw.github.com/alrra/browser-logos/master/opera/opera_48x48.png) | ![Safari](https://raw.github.com/alrra/browser-logos/master/safari/safari_48x48.png)
--- | --- | --- | --- | --- |
 ✔ | ✔ | IE9 + | ✔ | ✔ |


## Load

To use the directive, include the angular socialshare's javascript file in your web page:

```html
<!DOCTYPE HTML>
<html>
<body ng-app="app">
  //.....
  <script src="src/js/angular-socialshare.js"></script>
</body>
</html>
```

##Installation

####Bower

```bash
$ bower install angularjs-socialshare --save
```
####Npm

```bash
$ npm install angular-socialshare --save
```

_then [load](https://github.com/720kb/angular-socialshare#load) it in your html_

####Add module dependency
Add the 720kb.socialshare module dependency

```javascript
angular.module('app', [
  '720kb.socialshare'
 ]);
```

Call the directive wherever you want in your html page

```html
<a href="#"
socialshare
socialshare-provider="twitter"
socialshare-text="720kb AngularJS Socialshare"
socialshare-hashtags="angularjs, angular-socialshare"
socialshare-url="http://720kb.net">
Share me
</a>
```

##Usage
Angular socialshare allows you to use sharing options via `attribute` data

####Sharing Provider
You can set the social platform you want to share on using the `socialshare-provider=""` attribute.

#####Providers:

- [email](#email)
- [facebook](#facebook)
- [facebook-messenger](#facebook-messenger)
- [twitter](#twitter)
- [linkedin](#linkedin)
- [google](#google)
- [pinterest](#pinterest)
- [tumblr](#tumblr)
- [reddit](#reddit)
- [stumbleupon](#stumbleupon)
- [buffer](#buffer)
- [digg](#digg)
- [delicious](#delicious)
- [vk](#vk)
- [pocket](#pocket)
- [wordpress](#wordpress)
- [flipboard](#flipboard)
- [xing](#xing)
- [hackernews](#hacker-news)
- [evernote](#evernote)
- [whatsapp](#whatsapp)
- [viber](#viber)
- [skype](#skype)

Please use them all in lowercase (`socialshare-proivder="delicious"`)

##Doc

####Facebook

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
 	sharer, dialog, send		| socialshare-url="" 	 | page URL | false |		Set the url to share
 	dialog		| socialshare-text="" 	 | String |	 false	| Set the headline to share
 	dialog		| socialshare-description="" 	 | String |	 false	| Set the content to share
 	dialog		| socialshare-media="" 	 |	URL |	false | Set the media source to share
 	dialog, send		| socialshare-type=""	 | String('feed', 'send') | false |		Share via facebook feed dialog  - [info](https://developers.facebook.com/docs/sharing/reference/feed-dialog) or send dialog  - [info](https://developers.facebook.com/docs/sharing/reference/send-dialog)
 	dialog, send		| socialshare-via="" 	 |	String | false | 	Set the APP ID value
 	dialog	, send	| socialshare-to="" 	 |	String	| false | Set the to value
 	dialog		| socialshare-from="" 	 |	String	| false | Set the from to value
 	dialog, send		| socialshare-ref="" 	 |	String('comma,separated') | false |	Set the ref value
 	dialog, send		| socialshare-display="" 	 | String('popup') | false |	Set the display value
 	dialog		| socialshare-source="" 	 | URL | false |	Set the source value
 	dialog		| socialshare-caption="" 	 | String | false |	Set the caption to share
  dialog, send		| socialshare-redirect-uri="" 	 | URL | false |	Set the redirect URI


####Facebook Messenger 
(works only for `<a>` elements, it is a direct link)

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  sharer    | socialshare-url="" |  URL | page URL| Set the url to share


####Twitter

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
 	sharer		| socialshare-url="" |	URL | page URL|	Set the url to share
 	sharer		| socialshare-text="" | String	| false |	Set the content to share
 	sharer		| socialshare-via="" | String('username') | false |	Set the via to share
  sharer		| socialshare-hashtags="" |	String('hash,tag,hastag')| false   |	Set the hashtags to share


####Linkedin

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	        |	URL     | page URL  |	Set the url to share
	sharer		| socialshare-text=""           | String	| false     |	Set the title value that you wish to use
    sharer		| socialshare-description=""    | String    | false     |   Set the description value that you wish to use
    sharer      | socialshare-source=""         | String    | false     |   Set the source of the content

####Reddit

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
 	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
  sharer		| socialshare-subreddit="" 	 | String('technology')	| false |	Set the subreddit to share on

####Vk

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
 	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
	sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share

####Digg

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
	sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share

####Delicious

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
 	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
 	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
  sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share

####StumbleUpon

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
	sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share

####Pinterest

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
 	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
 	sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share

####Google (Plus)

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share

####Tumblr

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
  sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
  sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share

####Buffer

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
  sharer		| socialshare-via="" 	 | URL | false |		Set the buffer via

####Pocket

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text=""  | String	| false |	Set the content to share

####Flipboard

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text=""  | String	| false |	Set the content to share

####Evernote

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
 	sharer		| socialshare-url="" |	URL | page URL|	Set the url to share
 	sharer		| socialshare-text="" | String	| false |	Set the content title to share


####Hacker News

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text=""  | String	| false |	Set the content to share

####Wordpress

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text=""  | String	| false |	Set the content to share
  sharer		| socialshare-media="" | URL | false | Set the media url to share


####Xing

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
	sharer		| socialshare-url="" 	 |	URL | page URL|	Set the url to share
	sharer		| socialshare-text="" 	 | String	| false |	Set the content to share
	sharer		| socialshare-media="" 	 | URL | false |		Set the media url to share
  sharer		| socialshare-follow="" 	 | URL | false |		Set the Xing page url which will be then suggested to you to follow


####Whatsapp
(works only for `<a>` elements, it is a direct link)

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  sharer    | socialshare-url="" |  URL | page URL| Set the url to share
  sharer    | socialshare-text="" | String  | false | Set the content to share


####Viber
(works only for `<a>` elements, it is a direct link)

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  sharer    | socialshare-url="" |  URL | page URL| Set the url to share
  sharer    | socialshare-text="" | String  | false | Set the content to share


####Skype

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  sharer    | socialshare-url=""   |  URL | page URL| Set the url to share
  sharer    | socialshare-text=""  | String | false | Set the content to share

####Email

Method | Option | Type | Default | Description
------------- | ------------- | ------------- | ------------- | -------------
  mailto    | socialshare-subject=""   |  String | false | Set the subject for the email
  mailto    | socialshare-body=""  | String | false | Set the body content for the email
  mailto    | socialshare-to=""  | String | false | Set the Receiver / Receivers
  mailto    | socialshare-cc=""  | String | false | Set the CC / CCs for the email
  mailto    | socialshare-bcc=""  | String | false | Set the BCC / BCCs for the email


##Options

####Sharing Popup Size
you can set a specific Height or Width for the sharing popup using the `socialshare-popup-height=""` and `socialshare-popup-width=""` attributes

```html
<a href="#"
socialshare
socialshare-provider="reddit"
socialshare-url="http://720kb.net"
socialshare-text="Sharing it!"
socialshare-popup-height="800"
socialshare-popup-width="800">
Share with a bigger popup
</a>
```

####Sharing Event Trigger
You can choose to bind a different event trigger for showing up the sharer popup using the `socialshare-trigger=""` attribute (you can use any angular `element.bind()` event you want)

```html
<a href="#"
socialshare
socialshare-provider="reddit"
socialshare-text="Sharing on mouseover"
socialshare-trigger="mouseover">
Share me when mouse is over
</a>
```
or a set of

```html
<a href="#"
socialshare
socialshare-provider="reddit"
socialshare-text="Sharing on mouseover"
socialshare-trigger="focusout mouseleave">
Share me when focusout or mouseleave
</a>
```

##Globals
####Provider setup
Sometimes you may need to set default values for all the sharing buttons, here is how to setup this:

```javascript
.config(['socialshareConfProvider', function configApp(socialshareConfProvider) {

  socialshareConfProvider.configure([{
    'provider': 'twitter',
    'conf': {
      'url': 'http://720kb.net',
      'text': '720kb is enough',
      'via': 'npm',
      'hashtags': 'angularjs,socialshare,angular-socialshare',
      'trigger': 'click',
      'popupHeight': 800,
      'popupWidth' : 400
    }
  },
  {
    'provider': 'facebook',
    'conf': {
      'url': 'http://720kb.net',
      'trigger': 'mouseover',
      'popupHeight': 1300,
      'popupWidth' : 1000
    }
  }, //etc....put all the providers you want
  ]);
}])
```
*NB* if you define the provider settings, but then you change the option value by html attributes, the html attribute value will be the final one (the one that will be used)


####[Live demo](https://720kb.github.io/angular-socialshare)


##Contributing

We will be much grateful if you help us making this project to grow up.
Feel free to contribute by forking, opening issues, pull requests etc.

## License

The MIT License (MIT)

Copyright (c) 2014 Filippo Oretti, Dario Andrei

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
