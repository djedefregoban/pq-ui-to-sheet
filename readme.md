# ALWAYS UPDATE FIRST

# What to care about
1. Give a different session for each client to prevent manipulation

# Procedure
1. Email to the PQ Question Form
2. The form determines which PQ to send
3. Send Google Form to fill out the PQ
4. PQ automatically sent back to us in pdf to the correspond dropbox
5. if client doesn't do PQ within a certain amount of time, auto-follow-up

# Sender
1. Enter Client ID and PQ info on the website
3. Find the client on Notion using client ID
4. Create a task linked to the client specifying how pqs have been sent (timestamp! no check off!)
e.g.,
- Title
BOT: Send PQ - 3 PQ(s) have been sent (# set up date and dont check off the mark)
- Content
PA - Loviisa (General) - Sent
Spouse - Spouse or Common-partner of Loviisa (General) - Sent
Supporter - Shimmel - (PGP) - Received
...

2. Using PQ info, create entries based on each client and update pq status's form internal link
- create entry with taskid attached to it
5. Upload the JSON to the task

## Remarks
- Format the email
- Think about error checks more

# Watcher
1. Upon cathing an update, find the task using taskID coming from PQ info 
2. get the JSON in the task and look for the client using internal link
3. Update ifReturned to true from false (# will there be any situations where ifReturned is originally true?)
4. Send thank you email to the just completer (if the relationship is applicant, and the form has refusal etc. include those stuff into the email)
4. look through every ifReturned to check if every pq has been received (# make a function for this)
- if yes,
	1. using the task id, check off the mark of the task
	2. create another task linked to the client indicating every pq has been received (timestamp!)

- if no,
	do nothing?

# Reminder
1. look through bot tasks (if not checked off and timestamp has been more than a certain time amount)
2. send a remind email containig the pq status (using JSON!)

# Remarks
1. Date of completion

# Notes

1. Order matters for JD X

2. Italicize every help text X

3. Choose custom error X

4. Refactor and reorganize X

5. From, to filed no earlier than to X

6. Google JS API X

7. internal task id field on form X

8. ask for refusal or any letters depending on the question on pq later (only to PA only find out a way to do this)

9. Immigration History & Citizenship - send doc request upon any of the qeustions is answered yes

If you answer yes to any of the above questions, please provide: A scanned copy of the last document/letter received from Immigration, Refugees and Citizenship Canada

10. Applicaiton Details - send doc request upon the answer to this question (Have you ever submitted an application to any province in Canada?)

11. Copy and paste some important message from pq to the online form X

12. Travel History - more than six months indicator (automate it) X

13. Come up with no gap logic X

14. Thank you page

15. Readme page

17. Send a thank you email everytime one of them finishes with status

17. When PA submits PQ, send thank you email with status and document request if refusals and stuff.

18. PQ sending Front (relationship to PA field)

- dropbox change

- three digits for the client id

- task two times (sending and completion assigned to no one)

- booking link

## Check

1. Mandatory field or not?




git@github.com-djedefregoban:djedefregoban/pq-ui-to-sheet.git