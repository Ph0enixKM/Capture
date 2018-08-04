<div align="center">
  <img width="200" height="200" src="https://raw.githubusercontent.com/Ph0enixKM/Capture/master/logo.png">
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

## Configuration
Customization can be provided in a configuration object. Here is an example:
```js
let capture = new FileCapture({
  types: ['image', 'audio', 'video', 'text', 'zip', 'application']
  // These types are just an example... you can use any media type you want
  size: 5
  // Size is being given in megabytes (MB)
})
```

You can also create your own error behavior by editing error method of FileCapture instance.
```js
capture.error = value => {
  console.error(`File ${value} is incorrect`)
  // value parameter can be equaled to either 'size' or 'type' depending on which one is incorrect
}
```
That's all for now... more features are coming soon...
