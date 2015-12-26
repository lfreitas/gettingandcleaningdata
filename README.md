# gettingandcleaningdata

My repo for Coursera's Getting and Cleaning Data class project. The code's workflow is as follows:

1. Merges the training and the test sets to create one data set
2. Extracts only the measurements on the mean and standard deviation for each measurement 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. Note that nothing new is computed: only the columns with mean and standard deviation data are extracted

Variable names are defined from the following components:
* angle - for variables that start with angle, the rest of the variable describe the angle being measured
* timebody - time domain body signal
* frequencybody - frequency domain signal
* acceleration - acceleration measurement 
* jerk - jerk measurement
* gyroscope - measurements from a gyroscope
* x/y/z - axis for which the measurement is taken
* stdev - standard deviation
* mean - average of measurement
* meanfreq: weighted average of the frequency components to obtain a mean frequency
