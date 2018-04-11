---
layout: page
title: Audio Digitization Workflow using Audacity
menu: true
order: 9
lang: English
ref: audacity
permalink: /audacity
---

#### Set Preferences

**Devices**
* Set the host to core audio
* Set the playback device to Built-in Output
* Set the recording device to Benchmark 2.0
* Set the channels to 2 (Stereo)

![](../assets/img/audacity/image1.png)

**Quality**

* Go to the Quality tab.
* Set the sample rate at 96000 Hz
* Set the sample format to 24 bits
* Set sample rate converter to High Quality
* Set dither to None
* Set sample rate converter to Best Quality (Slowest)
* Set dither to None

![](../assets/img/audacity/image2.png)

#### Create a new audio track

**Path**

* Tracks>Stereo Track
* The two channel track will pop up.

**Name your audio track**

* Click on the top left tab with the downward pointing arrow for “Audio Track”
* Select Name
* Change the track name to the appropriate file name

![](../assets/img/audacity/image3.png)

#### Digitize tape
**Begin Recording**: Click the red circle button on the top left corner to capture. Hit record about 6 seconds before pressing play on the tape playback deck.

**Stop recording:** Click to yellow square on the top left corner to stop capture.

![](../assets/img/audacity/image4.png)

\*Monitor and listen to the recording while digitizing for squealing, dropout, clipping, and decibel levels.

#### Trim audio Track

**Trim beginning and end:**
* Use the magnifying glass icon at the top to zoom into your waveform.
* Click the cursor icon (I) to select.
* Place the cursor at the beginning of the waveform, a hand with a pointed finger should appear.
* Click and hold the mouse to drag the cursor over the area you want to trim.
* When you’ve highlighted the area, press delete on your keyboard.

![](../assets/img/audacity/image5.png)

![](../assets/img/audacity/image6.png)

\*Leave at least 6 seconds of time before the beginning and after the end of the recording.

#### Export audio track
**Path:**
* File>Export Audio

**Set export preferences:**
* Double check filename is correct.
* Set the target folder in the directory
* Set file type to other uncompressed files
* Set header to WAV (Microsoft)
* Set encoding to Signed 24-bit PCM
* Click save

![](../assets/img/audacity/image7.png)
