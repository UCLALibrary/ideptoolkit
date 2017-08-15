---
layout: page
title: MiniDV Transfer
menu: true
order: 6
---

## Equipment List

1. Sony Digital Video Deck Model HVR-M25AU (and AC power cord)
![](../assets/img/minidv/video_deck.png)

2. FireWire 800/400 9-Pin/6-Pin Cable
![](../assets/img/minidv/firewire.png)

3. Apple Thunderbolt to FireWire Adapter
![](../assets/img/minidv/firewire_adapter.png)
**For necessary tape repairs (4-6):**

4. 1⁄4” splicing tape
![](../assets/img/minidv/splicing_tape.png)

5. 1.4mm Phillips screwdriver
![](../assets/img/minidv/screwdriver.png)

6. Single edge razor or sharp scissors
![](../assets/img/minidv/razor.png)![](../assets/img/minidv/scissor.png)
<br>**For cleaning the video heads when they become clogged (7-8):**   

7. Lint-free swabs (for cleaning the video heads)
![](../assets/img/minidv/swabs.png)

8. Isopropyl Alcohol (99%) (for cleaning video heads)
![](../assets/img/minidv/alcohol.png)

## MiniDV Background

MiniDV is a video format introduced in 1995. Its small size and visual quality made it especially popular in the consumer and educational markets. Each tape holds about 13 GB for about one hour of video. Runtime is on average around 60 minutes if recorded at standard play (SP) or 90 minutes at long play (LP).

![](../assets/img/minidv/tape.png)

Like other DV format videotapes, the magnetic tape inside a MiniDV cassette is 1⁄4 inch wide so any repairs may be made with 1⁄4 inch splicing tape, typically used in audio work. While physical repairs are rarely required, repair techniques will be briefly reviewed at the end of this documentation.

![](../assets/img/minidv/tape2.png)

MiniDV tapes can be played in most DVCAM decks. The Sony deck you are receiving (Model HVR-M25AU) has a dual-size cassette mechanism that accepts both mini- and standard-sized DigitalMaster, DVCAM and DV video tapes. Note: certain Panasonic brand MiniDV tapes cannot be played on Sony decks.

The encoding stored on MiniDV tape can be Digital Video (DV), DVCAM or HDV. The video signal for all these formats is compressed or “lossy.” The audio signal for DV however is uncompressed. The sampling rate (number of audio samples per second) and the bit depth (number of bits used to carry the data in each sample of audio) can vary.

DV supports the following modes of linear pulse code modulated (PCM) audio:
* 4 channels at 12 bits with a 32 kHz sampling rate
* 2 channels at 16 bits with a 48 kHz sampling rate
* 2 channels at 12 bits 32 kHz mode
* 2 channels at 16 bits at 44.1 kHz sampling rate (similar to CDs)
Sampling rate:

![](../assets/img/minidv/sampling_rate.png)

DVCAM is a semi-professional version of DV and can play back at a faster rate.
HDV video is encoded with a H.262/MPEG-2 compression scheme and its stereo audio is encoded with the MPEG-1 Layer 2 compression scheme. The compressed audio and video are incorporated into an MPEG-2 transport stream.
The aspect ratio of a MiniDV video streams may either be standard (4:3) or widescreen (16:9):

![](../assets/img/minidv/ratio.png)

For this project we’ll be capturing the video data stream over a FireWire connection that will preserve the data in its more accurate form, including its original metadata. FireWire is also referred to as i.LINK. Transferring the stream over other traditional video outputs such as component or S-video out would alter the data.

![](../assets/img/minidv/s-video.png)

## Transfering MiniDV Content

The software you will use to transfer DV and DVCAM content is called AVCVideoCap. It’s a tool in Apple FireWire SDK Version 26, a software development kit for Mac OS. AVCVideoCap is an excellent candidate for MiniDV preservation because it transmits the raw data signals without applying any changes to the picture or sound. The resulting raw master file can be encoded to any variety of derivative files.

AVCVideoCap however will not capture HDV content. For tapes containing HDV, you will use is DVHSCap. Both workflows will be demonstrated below.

![](../assets/img/minidv/avcvideo.png)

**Connect cables and power:**
  1. Plug supplied power cord into the AC IN connector in the rear of the Sony HVR-M25AU DV deck. Plug the other end into your power source.
  2. Plug the FireWire 800/400 9-Pin/6-Pin Cable into the i.LINK jack in the rear of the DV deck. The 6-Pin connection will connect to the DV deck.
  3. Connect the FireWire 9-Pin connection to the Apple FireWire Thunderbolt adapter.
  4. Plug the Thunderbolt adapter into your MacBook Pro.
  5. Turn the DV unit on before turning on your computer.
      * Flip the power switch in the back of the unit to “ON”.
      * Press the power button in the front of deck.

**Prepare your MiniDV for transfer:**
  1. Ensure your MiniDV is set to “Safe Mode” so it cannot be accidentally recorded over.
  ![](../assets/img/minidv/mode.png)
  2.  Insert your MiniDV cassette. Gently but firmly push the tape into the tape door.
  3.  Rewind your tape if it isn’t already at the start of the recording.
  4.  Push “Play” and briefly review the aspect ratio, video and audio specifications. The LCD screen located on the front of the video deck will show the picture. Sound can be monitored with headphones plugged into the green headphone jack in the front of the deck. The audio sampling rate for your recording will automatically display on the LCD screen. Make sure the Audio Mode of the deck is set to match the original sampling rate of the recording. To do this go to: Menu>Audio Set>Audio Mode. Here you can adjust between 48 kHz or 32 kHz.

**Initiate transfer of DV/DVCAM:**
  1. For DV or DVCAM open capture software called AVCVideoCap by either:
      * Typing AVCVideoCap in Mac Spotlight search field or,
      * Goto: **Macintosh HD>Developer>FireWireSDK26>Applications>AVCVideoCap.app**

  2. Highlight the DV unit under listed devices
![](../assets/img/minidv/screenshot.png)
  3. Click on “Capture From Device.” Name your file and select a location on your hard drive to save the file to. Then click “Save.”
![](../assets/img/minidv/screenshot_2.png)
  4. Next, under recording mode, select “Tape Control,” then select “Continue.”
 ![](../assets/img/minidv/tape_control.png)
  5. The MiniDV will automatically begin playing and transmitting DV or DVCAM data. When complete the tape will automatically stop. If you wish to stop capture at any point, select “Abort Capture Now.” The resulting digital video file will have a .DV extension.
![](../assets/img/minidv/screenshot3.png)

**Initiate transfer of HDV content:**
  1. For HDV open capture software called DVHSCap by either:
      * Typing DVHSCap in the Mac Spotlight search field or,
      * Goto: **Macintosh HD>Developer>FireWireSDK26>Applications>DVHSCap.app**

  2. Choose “Capture from D-VHS.”
 ![](../assets/img/minidv/screenshot4.png)
  3. Name your project and select “Save” in the “Select Capture File” window. Select a location on your hard drive for capturing the video.
 ![](../assets/img/minidv/screenshot5.png)
  4. The MiniDV will automatically begin playing and transmitting HDV data. When complete the tape will automatically stop. If you wish to stop capture at any point, select “Stop Capture.” The resulting digital video file will have a .m2t extension.
![](../assets/img/minidv/screenshot6.png)

## Creating Streaming Files for Access

In addition to the raw .dv and .m2t files you will keep for preservation, you will create smaller mp4 files for streaming access.

1. Launch Adobe Media Encoder
  * Type Adobe Media Encoder into the Mac Spotlight search field or,
  * Go to: Launchpad > Adobe Media Encoder
2. Drag the .dv and .m2t files you want to transcode to the Queue.
![](../assets/img/minidv/access1.png)
3. Select each item in the queue, and under “Format” select H.264 from the drop-down list of video standards.
![](../assets/img/minidv/access2.png)
4. Under “Preset,” select “UCLA Library - Video - Streaming File.” The specifications for this preset are:
  * Video Stream: H.264/mp4 –AVC, SD, 480p
  * Audio Stream: 32 kHz/16-bit AAC
![](../assets/img/minidv/access3.png)
5. Under “Output File” click on the file name to select a location to save the files.
6. Repeat steps 3-5. Once you have a queue of files ready to be transcoded, click on the green play icon to start encoding. Ideally, you will process the files at the end of the work day and allow the processes to run overnight.
![](../assets/img/minidv/access4.png)

## Repairing MiniDV Tape

Occasionally a MiniDV tape will have to be repaired. The tape may have torn or the original cassette housing has an issue that prevents playback. Torn tape may be repaired with ¼” splicing tape. If the cassette housing is damaged, it can be replaced with a new blank MiniDV cassette.

![](../assets/img/minidv/New Picture.bmp)

1. Most Mini DV tapes have four small screws located on the underside of the casing. Using a small Phillips head screwdriver (approx. 1.4mm size), remove the four screws. Be careful not to let the tape inside unspool or get damaged. Place the screws in a secure location so they can be located easily when you’re done. If your tape does not have screws you will need to break the case open very carefully so the inside tape reels can be removed safely.
 ![](../assets/img/minidv/tape_repairing.png)   ![](../assets/img/minidv/tape2_repairing.png)
2. Then, carefully join the edges, securing with a small piece of splicing tape on the shiny side. Do not place any tape on the matte or dull surface as that side contains the recording. Carefully trim any splicing tape that hangs over the MiniDV tape edge. It is advised that you wear gloves when handling the tape to avoid damaging the recording surface (despite the poor example photo below).  
![](../assets/img/minidv/tape3_repairing.png)
<br>To prevent the tape from unspooling as you’re working, you may secure the hubs with a piece of tape:
![](../assets/img/minidv/tape4_repairing.png)
3. If the cassette body is damaged, you may transplant the reels into a new cassette housing that has been disassembled. Carefully remove the reels from the old cassette and place into the new shell. Remove any excess slack by hand winding the reels.
![](../assets/img/minidv/tape5_repairing.png)
4. Once repair is completed, place the tape cover in position and screw the casing shut to secure.
