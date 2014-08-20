MRI Bias Field Correction
=========================

This module is _NOT_ actively supported or maintained (See [#3401](http://na-mic.org/Mantis/view.php?id=3401)).
The associated code has been copied from Slicer [r23589](http://viewvc.slicer.org/viewvc.cgi/Slicer4?view=revision&revision=23589)

Note also the code will _NOT_ compile is its current state. The CMakeLists.txt
will have to be tweaked.

Description
-----------

Corrects 3D MRI images corrupted by MRI gain field effect.  This module removes the slow-varying intensity variation from a 3D image.  The output image has a higher contrast locally and the visualization and reading of the image are improved.  This is an important pre-processinbg step for image operations requiring intensity perfect images, such as the Expectation Maximization segmentation (see EMSegment module). The N3 and N4 methods are described in N4ITK: Nick's N3 ITK Implementation For MRI Bias Field Correction, Tustison N., Gee J., Insight Journal, 2009. http://hdl.handle.net/10380/3053 The Slicer code was contributed by Sylvain Jaume (MIT) for NA-MIC (http://na-mic.org).

Contributors
------------

Sylvain Jaume (MIT)

Acknowledgements
----------------

This work is part of the National Alliance for Medical Image Computing (NAMIC), funded by the National Institutes of Health through the NIH Roadmap for Medical Research, Grant U54 EB005149 (PI: Ron Kikinis).

Licensing
---------
Materials in this repository are distributed under the following licenses:

* All software is licensed under BSD style license, with extensions to cover
contributions and other issues specific to 3D Slicer. 
See License.txt file for details.
