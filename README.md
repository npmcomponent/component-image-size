*This repository is a mirror of the [component](http://component.io) module [component/image-size](http://github.com/component/image-size). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-image-size`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# Image Size

Get the dimensions of an image from a file input.

## Example

```js
var imageSize = require('image-size')

var input = document.querySelector('[input="file"]')
var file = input.files[0]

imageSize(file, function (err, size) {
  /*
  size = {
    width: xxxx,
    height: xxxx
  }
  */
})
````

## API

### imageSize(File, callback)

`callback` has the arguments `callback(err, size)`.
If `imageSize` is not supported, `size` wil be undefined.

### imageSize.supported === true || false

`imageSize` only supports:

- PNG and JPEG images
- Browsers with `FileReader`, `FileReader.prototype.readAsArrayBuffer`, and `Uint8Array`.

## License

The MIT License (MIT)

Copyright (c) 2013 Jonathan Ong me@jongleberry.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.