# Object-Detection
A repository containing a code to detect specific objects in images/videos.

# Source programs
* hogtrainfeatures.cpp : Extracts HOG features from a given set of images and stores them in a .xml file.
* hogtrainsvm.cpp : Uses the extracted HOG features and trains a SVM with them.
* hogobjectdetect.cpp : Uses the trained SVM to detect objects in images/livefeed.

# Dependencies
OpenCv (used version 3.0.1)

# Trial
```Code to be run in terminal```

$ cd Object-Detection

$ make train

$ ./output /PathToDirectoryContainingPositiveImages/ positive.xml

$ ./output /PathToDirectoryContainingNegativeImages/ negative.xml

$ make svm

$ ./output positive.xml negative.xml trainedsvm.xml

$ make all

$ ./output trainedsvm.xml /PathToTestImage

$ ./output trainedsvm.xml ```for livefeed detection```

