Introduction 
Robot Framework with Python for UI Automation

Pre-Requisite

1. Install Python
2. Install Pycharm IDE 
3. Install Selenium 
4. Install RobotFramework 
5. Install RobotFramework-SeleniumLibrary

To run test 
1. Prod = robot -d public -v environment:prod tests/
2. Staging = robot -d public -v environment:staging tests/ 
3. Specific file = robot -d public -v environment:prod tests/login.robot
4. Specific tag = robot -d public -v environment:prod --include=signup tests/

To see result
1.  go to /results
2.  click report.html

Scheduler using jenkins on local

Use this config

Build Trigger
TZ=Etc/GMT+8
0 9 * * *

Execute Shell
cd /your/paths/automation/folder
/your/paths/robot -d public -v environment:prod tests/
