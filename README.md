# estimatecron

Usage: ./estimatecron.c month crontab-file estimates-file

Program requires: a valid month argument, a valid crontab file 
and a valid estimates file. It uses these arguments to see:
  - the most frequently invoked command in the provided month
  - the total invoked commands
  - the maximum number of commands that executed simulataneously

Make file provided for compile
