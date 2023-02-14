# Node-RED-RESTful-API-and-Notifications

## Description
A set of workstations is reporting their state, to a remote monitoring system. 
<br>They update their state
through a RESTful API that the remote monitoring system offers.<br>
 use an event-driven application as Node-RED
 Monitor the state of a resource through RESTful Web Services

 <br>

 The workstations can be in any of the next states:
• IDLE
• WORKING
• ERROR

## Status : 'ERROR'

 <img src = '/image/error status.png'>
 <br>

## Status : 'IDLE'
 <img src = '/image/idle status.png'>

## Sending Mails
 <img src = '/image/sending_mail.png'>
 <br>

## workstation with 3 events  in Node-Red
 <img src = '/image/workstation 3 events.png'>

<br>

## Workstation state
 <img src = '/image/sending_mail.png'>


## Analyze the workstation state:

 For the event 1: every 4 minutes interval (as the condition is, greater than 3 minutes) in timestrap,<br> after the http request, if function finds out the payload is in idle state, only then it can send the email notification.<br>
For the event 2: every 2 minutes interval (as the condition is, greater than 1 minutes) in timestrap,<br> after the http request, if function finds out the payload is in ‘error’ state, only then it can send the email notification.<br>
For the event 3: every 3 minutes interval (as the condition is, greater than 2 minutes) in timestrap, <br>after the http request, if function finds out the payload is in idle state, only then it can send the email notification.<br>