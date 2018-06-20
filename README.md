# SLV Cropper
### JavaScript image cropper and region of interest selection.

### [Demo](https://salev.github.io/cropper)

Current version uses JQuery. _(It is planning to make a version with pure JS)_

This cropper was made with aim to have a module which could be easily incorporated into JavaScript application. So, no need to use GUI of the cropper. Nevetheless, you can take advantage of the GUI of the demo.

### Creation of the cropper object.
Global function __createSlvCropper(canvasSelector)__ builds and returns the cropper object.

Pass selector of your canvas as a parameter.


### Public methods of the cropper.
There are 5 public methods.

#### open(imgOrInput)
open method has one parameter which can be

1. image URL
2. image as an Image object
3. selector of <input type="file"> element.

#### save(callback)
returns resulting URL-encoded image through the provided callback.

#### onImageFileSelection(files)
_(use it when open method has a parameter of <input> element)_
example:
  onchange="slvCropper.onImageFileSelection(this.files)"

#### crop()
crops the image.

#### box()
draws a box.
