# jQuery.blogRSS (1.0)

* jQuery.blogRSS : v. 1.0
* Copyright (c) 2013 Zach Reed [Blue Tide Productions, LLC].
* License: GPL v3
* http://www.iamzachreed.com

## Demos

You can find a [Storenvy jQuery.blogRSS demo here](http://bluetidetest.storenvy.com/).

## Usage

First, include the jQuery library, jQuery.blogRSS javascript (<em>jQuery.blogRSS.js</em> or <em>jQuery.blogRSS.min.js</em>) and the jQuery.blogRSS CSS (<em>blogRSS.css</em>) on the page(s) where you want to use jQuery.blogRSS.

```html
	<script src="//ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
	<script src="jQuery.blogRSS.js" type="text/javascript"></script>
	<link rel="stylesheet" href="blogRSS.css" type="text/css">
```

Then, add a container div with an ID to your HTML so we can output jQuery.blogRSS somewhere.

```html
	<ul id="blogPosts"></ul>
```

Then, you will initialize jQuery.blogRSS. Put the following code before the closing tag of your body.

```js
	$(function () {
		$("#posts").blogRSS({
			feedURL: '', // required
			blogURL: '', // required
			ulContainerID: '', // required
			blogName: '', // overwrite RSS
			blogDescription: '', // overwrite RSS
		});
	});
```

Here is an example initialize:

```html
	<script type="text/javascript" charset="utf-8">
		$(function () {
			$("#posts").blogRSS({
				feedURL: 'http://blog.iamzachreed.com/rss',
				blogURL: 'http://blog.iamzachreed.com',
				ulContainerID: '#blogPosts',
				blogName: 'IAMZACHREED Blog'
			});
		});
	</script>
```

## Configuration Settings

*   **`feedURL`** - Your blog RSS/XML feed.
*   **`blogURL`** - Your blog URL.
*   **`ulContainerID`** - The ID of the container, which **must be** a UL element.
*   **`blogName`** - *optional* - Allows you to overwrite the RSS feed name.
*   **`blogDescription`** - *optional* - Allows you to overwrite the RSS feed cescription.

## Changelog

*   **jQuery.blogRSS : v. 1.0** (Oct 2013)

    First build of jQuery.blogRSS.

## More info, and contact
 *jQuery.blogRSS uses [Timeago](http://timeago.yarp.com/) to handle dates/times.*

[Email me](mailto:zreed@bluetideproductions.com) (or tweet me [@Bluetidepro](https://twitter.com/#!/bluetidepro)) if you have any questions about jQuery.blogRSS.