<div align="center">
<img src="https://github.com/sedeen-piip-plugins/StainAnalysis-plugin/blob/master/Images/PIIP_SRI_2.gif"  height="100" width="150"/>
</div>

<h1 align="center">RoiCropper Plugin</h1>
  
This plugin extracts region of interest from pathology slides given their coordinates in an .xml file (by a pathologist) and save them in a separated image. It aslo creates corresponding mask based on annotations in the region of interest.

<p align="center">
  <img src="https://github.com/sedeen-piip-plugins/RoiCropper/blob/master/Images/ROICroper_2.png"/>
</p>

<p align="center"> 
  <h6> <strong>Fig1.</strong> Annotated WSI with 6 selected ROI by the pathologist. Zoomed in ROI 1 in the annotated WSI.</h6>
</p>

## User Manual

1.	Open the WSI image in Sedeen Viewer. 
2.	Select the “RoiCropper” plugin from the pulldown list of Algorithms.

<p align="right">
  <img src="https://github.com/sedeen-piip-plugins/RoiCropper/blob/master/Images/ROICroper_1.png"/>
</p>

3.  Select “Region of Interest” in Parameters section (for example Region 55).

<p align="right">
  <img src="https://github.com/sedeen-piip-plugins/RoiCropper/blob/master/Images/ROICroper_3.png"/>
</p>

4.  Push the Run Bottom.

5.  Enter the name of whole slide image (for example 99797) and save it.

<p align="right">
  <img src="https://github.com/sedeen-piip-plugins/RoiCropper/blob/master/Images/ROICroper_4.png"/>
</p>

* The cropped region saves in the same path of original image with this naming format slideName_centreX_centreY_selectedRegion_crop.tif (for example: 99797_Region 55_23090_18015_crop.tif)

*	The corresponding mask saves in the same path of original image with this naming format slidename_selectedRegion_centreX_centreY_mask.tif (for example: 99797_Region 55_23090_18015_mask.tif)

*	The xml file which has extracted information of selected ROI from original image with this naming format slideName_selectedRegion_centreX_centreY_key.xml (for example: 99797_Region 55_23090_18015_key.xml).

## Authors
RoiCropper Plugin was developed by **Shiva Zaboli**, Martel lab at Sunnybrook Research Institute (SRI), University of Toronto and was partially funded by [NIH grant.](https://itcr.nci.nih.gov/funded-project/pathology-image-informatics-platform-visualization-analysis-and-management)

## Copyright & License

