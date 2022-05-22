# simple-modals

Simple, dependency free javascript modal

simple-modals is a **tiny** javascript and CSS modal library. It works very similarly to Bootstrap modals, without the need for jQuery or Bootstrap. In fact, simple-modals can be swapped out with Bootstrap modals without making any changes to your markup.

simple-modals exposes a single global method, `modal()`, that can be used to launch modals with JavaScript. However, the primary means of using simple-modals is through the use of HTML classes and attributes.

## Features

* Dependency free, no jQuery or Bootstrap

* Tiny
    * JS compressed, gzipped - 534 bytes
    * CSS compressed, gzipped - 593 bytes


* Responsive sizing
    * Modal size responds to viewport size
    * Modals never extend outside the viewport


* Optional size classes
    * modal-sm
    * modal-md
    * modal-lg
    * modal-xl


* Click delegation
    * Modals and buttons that are dynamically created will still work


* Swappable with Bootstrap
    * simple-modals uses the same class names and `modal()` method as Bootstrap, making it super simple to swap out as your project grows


## Install

```bash
npm install simple-modals
```


## Sample Code

```html
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>Simple Modal Demo</title>

        <link rel="stylesheet" type="text/css" href="modal.min.css">
    </head>
    <body>
        <button data-toggle="modal" data-target="#myModal">Launch Modal</button>
        <div id="myModal" class="modal modal-md">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-close">&times;</div>
                    <h1>My Simple Modal</h1>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                        sed do eiusmod tempor incididunt ut labore et dolore magna
                        aliqua.
                </div>
            </div>
        </div>
        <script type="text/javascript" src="modal.min.js"></script>
    </body>
</html>
```
