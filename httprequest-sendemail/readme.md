
# Use GET HTTP Method to request data from a specified resource and send an email with it

This example shows how to send an email to respective audience with requested data from a specified resource.

## Setup

1.  Go ahead and get started creating a blank workflow. If you need a refresher on how to get to this point, this [guide](https://docs.webmethods.io/integration/workflow_building_blocks/creating_first_workflow/#gsc.tab=0) can be a great introduction. 

2.  If you want the email to be sent periodically, you can do this by using polling triggers. In this example we will use Clock trigger and set an email to be send every week. Click on the small setting icon on start step and choose Clock trigger. Use the edit option to choose day and time and click Done. [PollingTriggerClock](https://github.com/marielaSAG/webmethodsio-examples/blob/master/httprequest-sendemail/PollingTriggerClock.png)

3.  Add the HTTP Request service in the canvas by drag and drop feature. This automatically connects with the Clock trigger. [ConnectHTTPRequest](https://github.com/marielaSAG/webmethodsio-examples/blob/master/httprequest-sendemail/ConnectHTTPRequest.png)

4.  Click on the small settings icon on the HTTP Request service to select HTTP Method and to add an URL. [HTTPRequest](https://github.com/marielaSAG/webmethodsio-examples/blob/master/httprequest-sendemail/HTTPRequest.png)

5.  To create custom HTML email template use Node.js service and add it in the canvas by drag and drop feature. Connect it to HTTP Request service. [AddNode.js](https://github.com/marielaSAG/webmethodsio-examples/blob/master/httprequest-sendemail/Nodejs.png) and [ConnectNode.js](https://github.com/marielaSAG/webmethodsio-examples/blob/master/httprequest-sendemail/AddHTML.png)

6.  We have a cool feature which is sending email where you can send the content to respective audience. Search for "send an email" and drag and drop the "Send an Email" service to canvas.

7.  Map the required fields in the Send an Email service. In this example we have mapped the address, subject and body.

8.  This completes the workflow and connects to stop step. [FinalWorkflow](https://github.com/marielaSAG/webmethodsio-examples/blob/master/httprequest-sendemail/FinalWorkflow.png)

9.  Check the email to review the results of the workflow.
