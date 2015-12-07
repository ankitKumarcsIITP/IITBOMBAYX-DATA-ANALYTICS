# IITBOMBAYX-DATA-ANALYTICS
edx-analytics-dashboard

This is the front end which renders the visulization of the summary data created at Result Store using a menu structure which divides the analysis of student data in three paradigms 'enrollment analysis', 'engagement' & 'performance'

IIT data analysis It has kept the essence of the openEdx edx-analytics architecture like creating listed query results at the back end as batch process & keeps the resultant data in the 'analytics' database of MySQL. The big data storage is hive storage as in edx. The places it diifers from the original edx are as follows

    Like edx data anlytics it is keeping big data (all logs) on hadoop cluster. Unlike edx data analytics this cluster is not installed on Amazon cloud, but is locally installed & managed.

    Instead of pushing the raw log files, it does some cleaning & send cleaned data to hadoop cluster. This stops repeated reading of entire log files where queries are generated.
    Edx data anlysis does map reduce on hadoop, here it is done on Sparks map reduce which is much faster.
    The front end uses R data analysis results & uses R library of visualization.
    The edx front end is also available as option.

