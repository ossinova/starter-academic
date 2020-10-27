---
title: Automate tasks using Cron jobs
subtitle: Scheduling repetitive tasks utilising crontab
date: 2020-10-27T15:00:25.088Z
draft: true
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
Do you manually perform repetitive tasks? Do you waste precious time doing daily tasks?

If you answered yes then cron will likely be a solution you can utilize to automate your tasks. 

Crontasks are fairly simple to create and can be run both locally (on Mac and Linux) or using a VM instance. A similar service can be used on Windows by utilizing task scheduler. 



For instance your daily task is to create a pivot table of yesterdays data based on a few dimesnions.  Rather than doing this manually in excel every single day, creating  Python script that does this for you can be achieved. Using cron this script can then be run in the background once every day at a  specified time. 

Assuming we have a Python script that reads a folder on our computer, checks for new files, triggers an action when a new file is found (creating a pivot), then saves the pivot to that excel file and moves it to a seperate folder. Added functionality can be made such as emailing the excel file, sending an email notification once the script has run and more. 



In the terminal we can simply setup a cronjob by writing:



`crontab -e `

The -e allows us to edit the crontab jobs. 



Crontabs are setup using a special formula

\* \* \* \*

Where the first * is for the minutes

the second for hours

then days, then months



If we want ot schedule it every hour we simply write 

\* \* \* \*