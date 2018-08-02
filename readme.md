<div align="center">
  <img width="200" height="200" src="https://github.com/Ph0enixKM/Capture/blob/master/logo.png">
  <br>
  <br>
</div>

# File Capture
This package solves a file drag and drop problem on client side with ease!

## Installation
```bash
$ npm i file-capture
```
All you have to do is to include capture.js script in your project
```html
<script src="node_modules/file-capture/capture.js"></script>
```
## Usage
Just initialize file capture object
```js
let capture = new FileCapture()
```
And create a DOM element for file drop
```html
<div class="file-capture"></div>
```
Now you can drag and drop files you want to be uploaded!
In order to get file data which has been uploaded you can use getFiles method
which returns a base64 of every uploaded file in one array
```js
let data = capture.getFiles()
```
That's all for now... more features are coming soon...