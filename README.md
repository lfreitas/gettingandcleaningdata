# gettingandcleaningdata

My repo for Coursera's Getting and Cleaning Data class project. The code's workflow is as follows:

1. Merges the training and the test sets to create one data set
2. Extracts only the measurements on the mean and standard deviation for each measurement 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. Note that nothing new is computed: only the columns with mean and standard deviation data are extracted

Measurement variable names are defined from the following components:
* angle - for variables that start with angle, the rest of the variable describe the angle being measured
* timebody - time domain body signal
* frequencybody - frequency domain signal obtained via Fast Fourier Transform
* acceleration - acceleration measurement 
* jerk - jerk measurement
* magnitude - magnitude of the three-dimensional signals
* gyroscope - measurements from a gyroscope
* x/y/z - axis for which the measurement is taken
* stdev - standard deviation
* mean - average of measurement
* meanfreq: weighted average of the frequency components to obtain a mean frequency

For example, frequencybodybodyaccelerationjerkmagnitudemean is the magnitude of jerk converted to a frequency domain signal for body acceleration. 

There are 86 measures included in the data set. The "subject" variable identifies subjects in the experiment, and the "actlabel" variable identifies the activity completed at the time.

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals. The magnitude of these three-dimensional signals were calculated using the Euclidean norm. 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals. These are flagged using the "frequency body" prefix. 

