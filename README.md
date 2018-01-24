# [3DSlicer]("https://slicer.org/") Plugin for calculating median signal intensities of segmentations

## Instructions:
1. Download/clone this repository
2. Add the following entry to the `SegmentStatistics.py` file in the Slicer application folder <br />(For Windows, it is: `C:\Program Files\Slicer....\lib\Slicer...\qt-scripted-modules)`: <br />
`ScalarVolumeModifiedSegmentStatisticsPlugin`
* (Instead of `  registeredPlugins = [LabelmapSegmentStatisticsPlugin, ScalarVolumeSegmentStatisticsPlugin,
                           ClosedSurfaceSegmentStatisticsPlugin]`
* It is now `  registeredPlugins = [LabelmapSegmentStatisticsPlugin, ScalarVolumeSegmentStatisticsPlugin,
                           ClosedSurfaceSegmentStatisticsPlugin, ScalarVolumeModifiedSegmentStatisticsPlugin]`)
3. Go into the folder `SegmentStatisticsPlugins`
4. Copy the `ScalarVolumeModifiedSegmentStatisticsPlugin.py` file into your Slicer application folder
5. Add the following line to the `__init__.py` file in the folder mentioned above: <br />
`from ScalarVolumeModifiedSegmentStatisticsPlugin import *`
6. Restart Slicer
7. Now you will be able to see the new plugin which includes the median in the computed stats (see following screenshot)

![Alt text](screenshot.png?raw=true "Screenshot")
