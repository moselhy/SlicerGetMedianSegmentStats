# [3DSlicer]("https://slicer.org/") Plugin for calculating median signal intensities of segmentations

## Instructions:
1. Download/clone this repository
2. Copy the `ScalarVolumeModifiedSegmentStatisticsPlugin.py` file into your Slicer application folder <br />(For Windows, it is: `C:\Program Files\Slicer....\lib\Slicer...\qt-scripted-modules\SegmentStatisticsPlugins)`
3. Add the following line to the `__init__.py` file in the folder mentioned above <br />
`from ScalarVolumeModifiedSegmentStatisticsPlugin import *`
4. Restart Slicer
5. Now you will be able to see the new plugin which includes the median in the computed stats (see following screenshot)

![Alt text](screenshot.png?raw=true "Screenshot")
