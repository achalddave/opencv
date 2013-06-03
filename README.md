This is a fork of the current latest stable version of OpenCV (2.5).  It
attempts to fix [a bug](http://code.opencv.org/issues/3064) with an undocumented
Haar detection function. 

It also comments the cascaded classifier source and changes the behavior of the
aforementioned undocumented function to fill `levelWeights` with (what seems to
be) a more sensible confidence, as described [in this
paper](http://eprints.utas.edu.au/8355/10/horton07chapter6.pdf) (bottom of the
first page). 

Most changes are located in `modules/objdetect/src/cascadedetect.cpp` and
`modules/objdetect/src/cascadedetect.hpp`.
