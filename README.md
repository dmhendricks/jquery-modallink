[![Author](https://img.shields.io/badge/author-Daniel%20M.%20Hendricks-lightgrey.svg?colorB=9900cc )](https://www.danhendricks.com)
[![Latest Release](https://img.shields.io/github/release/dmhendricks/jquery-modallink.svg)](https://github.com/dmhendricks/jquery-modallink/releases)
[![Bower](https://img.shields.io/bower/v/file-icon-vectors.svg)](https://github.com/dmhendricks/file-icon-vectors)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/danielhendricks)
[![GitHub License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://raw.githubusercontent.com/dmhendricks/jquery-modallink/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/url/https/github.com/dmhendricks/jquery-modallink.svg?style=social)](https://twitter.com/danielhendricks)

# jQuery Modal Link

A simple jQuery plugin to display any external links into a modal popup via iframe. Original code by [BrightSpark](https://github.com/brightspark-est).

[Demo](https://www.jqueryscript.net/demo/Simple-iFrame-Modal-Plugin-With-jQuery-modallink/) | [Original Source](https://www.jqueryscript.net/lightbox/Simple-iFrame-Modal-Plugin-With-jQuery-modallink.html)

### Bower Installation

```
bower install jq.modallink --save
```

## Usage

#### Link to Library

```
<link rel="stylesheet" href="jquery.modalLink.min.css">
<script src="//code.jquery.com/jquery.min.js"></script>
<script src="jquery.modalLink.min.js"></script>
```

#### Create Modal Toggle Link

```
<a href="iframe.html" class="modal-link">Open</a>
```

#### Initialize Modal Link

```
$(".modal-link").modalLink();  
```

#### External Link Example

```
<button class="btn-click-me">click me</button>

$(".btn-click-me").click(function () {
  $.modalLink.open("iframe.html", {
    // options here
  });  
});
```

#### Plugin Options

```
$(".modal-link").modalLink({
  height: 600,
  width: 900,
  showTitle: true,
  showClose: true,
  overlayOpacity: 0.6,
  method: "GET",
  disable<a href="https://www.jqueryscript.net/tags.php?/Scroll/">Scroll</a>: true,
  onHideScroll: function () { },
  onShowScroll: function () { }
});   
```

#### Actions

```
// close the modal
$.modalLink("close")

// open the modal
$.modalLink("open")
```

#### Events

```
$(".modal-link").on("modallink.close", function() {
  // do something on close
});
```

## Change Log

Release changes are noted on the [Releases](https://github.com/dmhendricks/jquery-modallink/releases) page.

#### Branch: `master`

* Initial version

## Screenshot

![Modal Screenshot](https://raw.githubusercontent.com/dmhendricks/jquery-modallink/master/demo/screenshot-1.png)
