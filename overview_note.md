# Module Overview

## Sender
1. Enter Client ID and PQ info on the website
2. Find the client on Notion using client ID
3. Create a task linked to the client specifying how pqs have been sent (leave timestamp! dont check off done!)

e.g.,
- Title
BOT: Send PQ - 3 PQ(s) have been sent (# set up date and dont check off the mark)
- Content
PA - Loviisa (General) - Sent
Spouse - Spouse or Common-partner of Loviisa (General) - Sent
Supporter - Shimmel - (PGP) - Received
...

4. Using PQ info, create entries based on each client and update pq status's form public link
- create entry with taskid attached to it

5. Upload the JSON to the task
6. Send email containing PQ links

## Watcher
1. Upon catching an update, find the task using taskID coming from PQ info
2. get the JSON in the task and get the client page
3. Update ifReturned to true
4. Update the JSON file

Paths:
4. Send document request email if the completer is PA
4. look through every ifReturned to check if every pq has been received (# make a function for this)
- if true,
	1. using the task id, check off the mark of the task
	2. create another task linked to the client indicating every pq has been received (timestamp!)
	3. Send booking email
	4. Send PQ documents for their review

- if false,
	done

## Reminder
1. look through bot tasks (if not checked off and timestamp has been more than a certain time amount)
2. send a remind email containig the pq status (using JSON!)

## Email formats
- LMIA email content

PLEASE PROVIDE DOCUMENTS (BELOW) - SCANNED COPY

Any advertising that you have done

Article of incorporation for your business

Proof of Business Registration from CRA

# Notes

18. PQ sending Front (relationship to PA field)

- dropbox change

- three digits for the client id

- task two times (sending and completion assigned to no one)

- booking link

# Todos

1. change the dropbox credential
2. Fix the front so that it'll be bugless
3. Beautify the email




# Form

- Mandatory fields

- Which questions to know which documents to request (DO THIS?)

# Dropbox

- Dropbox access (JD)

# Notion (Front end)

- validate the email address before putting into the master list (https://verifalia.com/validate-email)

# Improvements

- Document templates

- More PQs
