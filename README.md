# browser.report

💪💪💪Layout library for browser based reporting.

We can't control browser's page breaking when contents overflowed. So, this library splits overflowed contents, and breaks the page on DOM tree.

## Examples

<img src="browser.report/example1/example1-on-browser.png">

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="../report.css">
        <style>
            #fruit-name-label {
                border: 1px solid black;
            }
        </style>
    </head>
    <body>
        <div class="br-content br-a4-portrait br-hide">
            <div class="br-field-group">
                <div class="br-field">
                    <div id="fruit-name-label" class="br-label">Name</div>
                    <div id="fruit-name-value" class="br-value">Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana BananaBanana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana Banana</div>
                </div>
            </div>
        </div>
        <script src="../report.js"></script>
    </body>
</html>
```