# estimatecron

Usage: ./estimatecron.c month crontab-file estimates-file

Program requires: a valid month argument, a valid crontab file 
and a valid estimates file. It uses these arguments to see:
  - the most frequently invoked command in the provided month
  - the total invoked commands
  - the maximum number of commands that executed simulataneously

Example crontab file:
- - - - - - - - - - - - - - - - - - - -
# execute a command at 3AM every day
0 3 * * *     daily-backup
#
# execute a command at 4:15AM every Sunday
15 4 * * sun   weekly-backup
#
# start thinking about the project....
0 10 22 7 mon  deep-thought
#
# submit my project automatically, just in case I forget!
59 16 16 8 *   submit-project
#
# mail out a monthly newsletter
0 2 1 * *      send-monthly-newsletter
- - - - - - - - - - - - - - - - - - - -

Example estimates file:
- - - - - - - - - - - - - - - - - - - -
# format:  command-name   minutes   
weekly-backup             6
daily-backup              2
send-monthly-newsletter   10
submit-project            1
deep-thought              600
Traverses the crontab file 
- - - - - - - - - - - - - - - - - - - -


