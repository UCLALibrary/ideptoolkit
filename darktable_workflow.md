---
layout: page
title: darktable (Print/Image)
menu: true
order: 10
lang: English
ref: darktable
permalink: /darktable
---

#### Open laptop and darktable
1. Start up and log in to laptop
2. Connect camera to laptop via USB3 tether cable
3. Open darktable
	* Confirm darktable recognizes camera Nikon DSC D810 (the camera must be turned on)
	* If camera is not recognized, navigate to the "lighttable view", expand the "import" menu in the top left of the window, and select "scan for devices"
	* Once camera appears, select "tethered shoot"
	![](../assets/img/darktable/darktable1.png)
	* Or, navigate to tethering view by hovering over "other" tab dropdown, then click "tethering"
	![](darktable2.png)
4. Create a new roll by entering a "jobcode" in the session dropdown panel. In darktable, each session will be a unique roll.
	* click on the "session" dropdown > type in the "jobcode"
	![](darktable3.png)
	* Name the session you are in with a date (recommended), or collection name and session number

### START CAPTURE

#### Test flash settings
1. Take an image, ideally using the remote shutter release or button available in darktable to prevent camera shake.
	* click the eye icon in the live view panel to toggle view on laptop screen
	![](darktable5.png)
	* Make sure 'camera settings > properties > program' is set to "M" for manual exposure. Adjust settings as needed.
	* In the camera settings panel, click "capture image(s)"
	![](darktable4.png)
2. Review image in darktable in the darkroom tab
	* Zoom into the image – are things in focus?
	* Look at histogram graph in the top right – is the image too dark or too light?
  * Histogram should be evenly distributed without too much information skewing right or left. If the hills are too far to the right, the image will appear darker than it should be. If hills are too far to the left, the image will appear lighter than it should be.
  * Adjusting the output in the battery pack may be needed at this point to either provide more or less light, depending on histogram. Adjust and troubleshoot until histogram looks evenly distributed.

#### Take a photo with color reference target
1. Reference target photo should be taken at the beginning of the each session when the lighting conditions or exposure settings have changed, or when the materials that are being shot are very different in size or type.
2. Place the target directly on the surface of the object to be digitized.
3. Reference target should be photographed straight on with the same lighting that will be used to illuminate the materials. Avoid shadows and do not obscure color swatches on target when holding target in front of materials.

#### Continue taking images and checking them in darktable
1. Continually compare images to corresponding histogram to ensure evenly distributed light
2. Keep an eye on battery levels on camera, lighting battery pack, laptop and flash remote

### Post Capture Breakdown
* **Never unplug flash heads from battery pack while battery pack is on**
* Turn off battery pack and then discharge remaining power using white button on the top of battery pack
* Keep white portion of softboxes clean and white for maximum use

### Post Capture Processing
During capture, the images in darktable will be in a RAW format. The best way to implement post capture changes is to do so to the .RAW file. Once all changes/edits have been made, the files can be exported in TIFF or JPEG format making them more functional across applications.

Processing includes the following:
1. Crop/Skew
  * For master images leave ⅛" around image
  * Use functions in darktable to straighten image if necessary
2. Color correction
  * Use XRite Color Checker software and reference images to correct color (see section about XRite Color Checker)
3. Create derivatives
  * Export master files in TIFF format, and export other derivatives as needed
   ![](darktable6.png)
  * Choose resolution to export at (300 - 600 ppi)
4. Back up work
  * It is recommended that work be mirrored on a hard drive when possible

File Naming:
darktable renames files at export. Define filenames in the "target storage" field. Pre-defined variables can be used as templates. A list of options is available in the darktable user manual section 2.3.12.1
![](darktable7.png)

### File Specifications at a Glance
* File format for master images: TIFF
* File format for derivatives: JPEG or PDF/PDFa
* Output resolution: 300 - 600ppi
* Bit depth: 8 bits per channel (24 bit total)
* Color: RGB highlights should not exceed 250 - 250 - 250, shadows no lower than 5 - 5 - 5, check histogram for this information
* Color space: sRGB or Adobe RGB 1998

### Image Quality Control Tips
The following is a simplified list of quality control checkpoints to consider during and after digitization. Check for the following:
* Format  - each image is in the correct format.
* Compression - files are compressed or left uncompressed per the project instructions
* Bit Depth - correct bit depth has been selected (check metadata in darktable)
* Resolution - 300 - 600 ppi, 400 ppi and up for OCR purposes (check metadata in darktable)
* Color - output color closely matches true color of the materials, correct color mode has been selected.
* Orientation - all images are oriented correctly, no distortion or proportion irregularities.
* No physical matter - no dirt, dust, etc. obstructing the view of the item.
* No digital artifacts - no glare, no lens flare etc.
* Page order - keep track of the page order while scanning and also check a sample size at the end of the scanning process.
* Cropping - images are properly cropped (default = 1/8 inch on all sides) or per the project instructions.
* File naming and folder structure follows consistent protocol or project instructions

### File Naming & Folder Structure

**Best Practices**

Well-organized structures and file names make it easier to keep track of your data. When naming and organizing files, you should be consistent and descriptive to make it possible to find specific data and know what the files contain and what their status is. Set up a clear directory structure that includes information like the project title, a date, and some type of unique identifier. Individual directories may be set up by date, researcher, experimental run, or whatever categories make the most sense for you and your research needs.

**Structuring Data**

Think carefully about how best to structure your data from the very earliest stages of your project. This is particularly important when you have a number of collaborators, or are planning on sharing your data. Think about whether you need a deep or shallow hierarchy. **Aim for a shallow hierarchy**.

Some examples of data structures include organization by:
* types of data (text, images, sound files, etc.)
* research activities (interviews, surveys, focus groups, etc.)
* material (data, documentation, publication, etc.)

**File Naming**

For file naming conventions, see the "File Naming & Organization" Guide: [https://uclalibrary.github.io/ideptoolkit/filenaming.html](https://uclalibrary.github.io/ideptoolkit/filenaming.html)

**Other tips**

Include in the directory a `README.txt` file that explains your naming format along with any abbreviations or codes you have used. This documentation will be helpful both during the project or experiment, and also in the future.

### Color Correction
**Color Correction Using XRITE and Color Checker**

Note: Read Me documentation that comes with software provides step by step instructions.
 - Insert disc and install software, or install latest version from file download at from xritephoto.com (only the first time)
 - Using darktable, export the image containing the Color Reference Target as a .TIFF file
 - Open the ColorChecker Passport software, navigate to the ICC-TIFF panel, and drag in the TIFF image
 - The software should automatically find the color swatches
 - Click "Create Profile" to save,  name appropriately so that it can be recognized as a reference file for the corresponding session. A new profile will be created for each session.
 - Software will save as .ICC file, likely to /User/yourname/Libary/ColorSync/Profiles
 - Copy this .ICC file to $HOME/.config/darktable/color/in. $HOME represents your home directory.
 - Restart darktable and navigate to the darkroom tab > color group > input color profile
	* The profile you created should show up in the input color profile list drop down. Apply profile to the selected image
* If the image appears dark after applying the profile, click "more modules" > "unbreak user input profile"
![](darktable12.png)
	* change mode to "gamma" from the drop-down menu
	* set linear value between 0.0 and 0.1, making sure that full range of shadows and highlights remain intact in the histogram
	* set gamma value to 0.45, adjust if needed to make sure that full range of shadows and highlights remain intact in the histogram

- Apply profile to all images that were shot under the same lighting condition by using the "history stack"
![](darktable11.png)
	 - With the Color Reference Target image still selected, navigate to the lighttable tab and expand the "history stack" module
	 - Click "copy" > select all edits relevant to the entire session of images > click "ok"
	 - Select the entire session of images, and click "paste" in the history stack module

**White Balance Using darktable**
Note: this method adjusts image white balance but does not correct color. This step is not necessary if an XRITE .ICC profile is applied, and serves as a last resort for editing (better than nothing!)
 - Select the image with the Color Reference Target
 - Navigate to the darkroom tab > basic group > white balance > preset > click the dropdown to select "spot"
 ![](darktable10.png)
 - Within the image, select an area from the light grey square color palette, below the "colorchecker" text. The white balance is calculated based on the selected area.
 ![](darktable8.png)
 ![](darktable9.png)
 - Review the resulting edit in darktable -- is the image too warm or cool? Do colors accurately represent the material? If not, repeat the previous steps using a different selection of grey area from the color palette.
 - Apply white balance edit to all images that were shot under the same lighting condition by using the "history stack"
![](darktable11.png)
	 - With the white balance-corrected image still selected, navigate to the lighttable tab and expand the "history stack" module
	 - Click "copy," then select the white balance edit and any other color correction edits that may be relevant to the entire session of images
	 - Select the entire session of images, and click "paste"
