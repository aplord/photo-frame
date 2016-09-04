# photo-frame
This suite of Python software controls an internet-enabled photo frame. Here’s what it does:

1. Runs on a Raspberry Pi which is attached to a screen of some sort. Together, the RPi and screen are a photo frame. The software synchronises to a local SD card relevant photos and photo folders contained in the OneDrive repository, using standard OneDrive sync functions called using the standard OneDrive python API. Photos synchronised in this way are displayed cyclically on the screen.

2. The software envisages that the photo frame may be one of many which draw photos from the OneDrive repository. Each frame may draw a different set of pictures from the repository, in accordance with a photo frame-specific parameter file stored on OneDrive. The parameter file also controls additional display logic, such as transition styles and timing, and weighted preference for random display frequency for each photo or group of photos.

3. As well as displaying the photos, the software displays additional information, for example alerts for extreme weather and for hourly chimes. The photo frame-specific parameter file also controls display characteristics for these elements.

4. The photo frame also takes instructions from a Domoticz home automation server. This allows the frame screens to be turned on/off according to whatever logic is contained on the Domoticz server. Therefore the photo frame will not display images when “off”, although it will continue to sync with OneDrive at all times.
