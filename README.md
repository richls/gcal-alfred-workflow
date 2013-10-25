"View date in Google Calendar" workflow for Alfred 2
====================================================

An [Alfred 2](http://www.alfredapp.com) workflow for viewing a particular date in Google Calendar. Also functions as a simple date calculator.

I use the "`date`" keyword as a trigger for this action in Alfred 2.  You can change it to "`gcal`" 
or whatever suits your fancy.  By default, dates are in US MM/DD/YY format, but you can change this by following 
the directions under [Date Formats](#date-formats) below.

##Uses
* Enter a date and press Enter to jump to that date in Google Calendar.  While the Alfred window is open, it will show you the complete date and day of week for that date.

    > For example: `date 12/25` or `date 12/25/13` or `date 12/25/2013` will all open the Google Calendar page containing December 25, 2013.

* Use "+" or "-" after the date to navigate by days (d), weeks (w), months (m), or years (y). 
    > For example: `date 12/25/13+2w` will show you the Google Calendar page for Wednesday, January 8, 2014.
* You can use "+" or "-" without a date to navigate from the current date (today).
    > For example: `date +1w` will show you the Google Calendar page for the day one week from today;
    > `date -1` or `date -1d` will show you yesterday, and `date +2m` will show you two months from today. 

##Date Formats
By default, the current code is set to use US-style dates, in the format "MM/DD/YY".  

You can change it to use "DD/MM/YY" by changing the `$date_format="US";` line to `$date_format="UK";` 
(or any other value), and you can use a different separator character by changing `$date_sep="/";` to suit your fancy.
