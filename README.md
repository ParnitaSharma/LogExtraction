# LogExtraction
My first approach towards solving this problem statement “Log Extraction Project” was to
understand the significance of this use case and then creating a development approach to
accomplish the desired output.
I chose C# to execute this Use case, I estimated 8 hours to
complete it. My estimates were taken considering following small steps:
1) Taking inputs from CLI to exe file
2) Converting input into desired format
3) Traversing the log files
4) Reading the log files
5) Selecting log lines satisfying the condition (given in the input)
6) Fetching the data
7) Displaying the data
My Approach:
In the main part of the program, I have taken inputs from CLI and have stored in args[0]
(time), args[1](time), args[2](path). The time that I am receiving is of ‘String time’ and to
change it into ‘DateTime’ format, there are two methods written: addZero() and
DateTime.ParseExact().
Now, with the third input, which is the path of the folder, where all the log files are stored.
Directory.GetFiles() is used to search for file starting with ‘LogFile’ in the given folder path.
After that I have tried to traverse each file using foreach loop. In the next step I am fetching 
the time written in the starting of the log lines and then converting the ‘String’ type time
into DateTime ISO 8601.
After traversing each log line, the data against the matched time stamp is getting stored in
the variable named ‘data’ and then I have printed this ‘data’ as it is our desired output.
