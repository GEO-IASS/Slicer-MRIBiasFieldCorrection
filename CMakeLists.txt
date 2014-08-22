cmake_minimum_required(VERSION 2.8.9)

project(MRIBiasFieldCorrection)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://wiki.slicer.org/slicerWiki/index.php/Documentation/Nightly/Modules/MRIBiasFieldCorrection")
set(EXTENSION_CATEGORY "Legacy.Filtering")
set(EXTENSION_CONTRIBUTORS "Sylvain Jaume (MIT)")
set(EXTENSION_DESCRIPTION "Corrects 3D MRI images corrupted by MRI gain field effect. This module removes the slow-varying intensity variation from a 3D image. The output image has a higher contrast locally and the visualization and reading of the image are improved. This is an important pre-processinbg step for image operations requiring intensity perfect images, such as the Expectation Maximization segmentation (see EMSegment module). The N3 and N4 methods are described in N4ITK: Nick&#39;s N3 ITK Implementation For MRI Bias Field Correction, Tustison N., Gee J., Insight Journal, 2009. http://hdl.handle.net/10380/3053 The Slicer code was contributed by Sylvain Jaume (MIT) for NA-MIC (http://na-mic.org).")
set(EXTENSION_ICONURL "")
set(EXTENSION_SCREENSHOTURLS "")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(MRIBiasFieldCorrection)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
