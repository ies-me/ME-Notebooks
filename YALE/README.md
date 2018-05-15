Normalized YALE Face Database downloaded from http://vismod.media.mit.edu/vismod/classes/mas622-00/datasets/

All content but the `centered` directory was discarded.

Original readme:

# The normalized yale face database

Originally obtained from [the yale vision group](http://cvc.yale.edu/projects/yalefaces/yalefaces.html) [defunct link].
The location of they eyes in each frame was picked manually and used to
normalize the head by rotation and cropping.
The normalization matlab code is available in the tree.
The data files are either in PGM format (not recommended for image processing
as these are scaled in intensity to cover 0..255) or written out as an array of
floats.
The size of float files is the same as that of the pgm files.

    yalefaces.tar.gz       The original dataset from YALE.tar.gz
    faces/                 The original dataset in PGM format.
    matlab/                Code used to process the original YALE dataset
    rotated/               Faces rotated so eyes are aligned horizontally
    centered/              Rotated faces cropped and middle of eyes centered.
    unpadded/              Centered faces cropped out
    supported/             Unpadded faces shrunk and outline blanked out
    eigfaces/              Unpadded faces gone through SVM as arrays of floats
    eigfaces-for-your-vie  The above as PGMs (not suitable for processing as
                           they have undergone rescaling by matlab)
    eyelocs.mat            Locations of eyes
    eyedistances.dat       Distances between eyes
    support-trapezoid.pgm  The support map used
    support.pgm            An alternative support map which preserves more pixels
    eigenvalues.dat        The computed eigenvalues

In addition, you might find pgmRead.m and pgmWrite.m useful.

Browse the directory.

Download the directory as a tgz.

