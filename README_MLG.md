# Evaluation of Activity Monitor Data
## Reproducible Data Peer Assessment 1 
Submitted by Miranda L. Gardner

## Introduction

It is now possible to collect a large amount of data about personal
movement using activity monitoring devices such as a
[Fitbit](http://www.fitbit.com), [Nike
Fuelband](http://www.nike.com/us/en_us/c/nikeplus-fuelband), or
[Jawbone Up](https://jawbone.com/up). These type of devices are part of
the "quantified self" movement -- a group of enthusiasts who take
measurements about themselves regularly to improve their health, to
find patterns in their behavior, or because they are tech geeks. But
these data remain under-utilized both because the raw data are hard to
obtain and there is a lack of statistical methods and software for
processing and interpreting the data.

This assignment makes use of data from a personal activity monitoring
device. This device collects data at 5 minute intervals through out the
day. The data consists of two months of data from an anonymous
individual collected during the months of October and November, 2012
and include the number of steps taken in 5 minute intervals each day.

## Data

The dataset for this assignment can be downloaded here:

* Dataset: [Activity monitoring data](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip) [52K]

The variables included in this dataset are:

* **steps**: Number of steps taking in a 5-minute interval (missing
    values are coded as `NA`)

* **date**: The date on which the measurement was taken in YYYY-MM-DD
    format

* **interval**: Identifier for the 5-minute interval in which
    measurement was taken




The dataset is stored in a comma-separated-value (CSV) file and there
are a total of 17,568 observations in this
dataset.

### Load and examine the data

1. Read the data into R.

2. Process/transform the data (if necessary).


### What is mean total number of steps taken per day?

Note: Missing values are ignored for the next two parts of the assignment.

1. Group data by date and summarize to calculate the mean, median and total number of steps taken per day.

1. Make a histogram of the total number of steps taken each day.

2. Report the **mean** and **median** total number of steps taken per day.


### What is the average daily activity pattern?

1. Group data by interval and calculate the average number of steps taken across all days.

1. Construct a time series plot of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all days (y-axis).

2. Report which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps.


### Imputing missing values

Note that there are a number of days/intervals where there are missing
values (coded as `NA`). The presence of missing days may introduce
bias into some calculations or summaries of the data.

1. Calculate and report the total number of missing values in the dataset.

2. Devise a strategy for filling in all of the missing values in the dataset. In this case, the mean number of steps over the 5 min time interval was imputed. 

3. Impute the missing values into the original dataset and report the new data.

4. Generate a histogram of the total number of steps taken each day. Calculate and report the **mean** and **median** total number of steps taken per day. Do these values differ from the estimates from the first part of the assignment? What is the impact of imputing missing data on the estimates of the total daily number of steps?


### Are there differences in activity patterns between weekdays and weekends?

For this part the `weekdays()` function may be of some help here. Use
the new imputed dataset generated above.

1. Create a new factor variable in the dataset with two levels -- "weekday" and "weekend" indicating whether a given date is a weekday or weekend day.

1. Make a time series plot of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all weekday days or weekend days (y-axis). The plot should look something like the following, which was created using **simulated data**:

![Sample panel plot](instructions_fig/sample_panelplot.png) 


**Your plot will look different from the one above** because you will
be using the activity monitor data. 


```
