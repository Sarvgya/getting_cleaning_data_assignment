# Project(Getting and Cleaning Data)

Repository was created in the following ways:-
* Download and unzip the data file into your working directory.
* Download the R source code into your R working directory.
* Execute R source code to generate tidy data file.
### Data
The variables in the data X are sensor signals measured with waist-mounted smartphone from 30 subjects. The variable in the data Y indicates activity type the subjects performed during recording.

### New dataset
The new generated dataset contained variables calculated based on the mean and standard deviation. Each row of the dataset is an average of each activity type for all subjects.

### Steps are as per the question.
1. Merges the training and the test sets to create one data set using rbind() function.
2. Only the measurements on the mean and standard deviation for each measurement by using grep command to get column indexes for variable name contains "mean()" or "std()"
3. Uses descriptive activity names to name the activities in the data set by convert activity labels to characters and add a new column as factor.
4. Appropriately labels the data set with descriptive variable names and giving the selected descriptive names to variable columns.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Finally, use pipeline command to create a new tidy dataset with command group_by and summarize_each in dplyr package.
