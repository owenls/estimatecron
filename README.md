#Author 1: Owen Smith -> https://github.com/owenls

#Author 2: John Lumagbas -> https://github.com/Syncline-blip

#estimatecron

Usage: ./estimatecron.c month crontab-file estimates-file
Make file provided for compile

Program requires: a valid month argument (0-11 or 3-char i.e apr or jun),
a valid crontab file and a valid estimates file.
Estimatecron uses these files and arguments to see:
  - the most frequently invoked command in the provided month
  - the total invoked commands
  - the maximum number of commands that executed simulataneously

Crontab File

- crontab file provides the commands to be executed and times

Estimates File

- estimates file provides execution times for the commands

