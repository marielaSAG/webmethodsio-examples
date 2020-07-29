
# Use GET HTTP Method to request data from a specified resource and send an email with it

This example shows how to send an email to respective audience with requested data from a specified resource.

## Setup

1. Go ahead and get started creating a blank workflow. If you need a refresher on how to get to this point, this [guide](https://docs.webmethods.io/workflow-building-blocks/creating-first-workflow) can be a great introduction. 

2.  Add the HTTP Request service in the canvas by drag and drop feature. This automatically connects with the start of the step.![AddHTTPRequest](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/adddropbox.PNG)

3.  Click on the small settings icon on the HTTP Request service to select HTTP Method and add an URL. ![HTTPRequestAction](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/dropboxaction.PNG)

4.  Add the Dropbox connection details to create the connection to dropbox. We can use the automatic default feature to connect where the webmethods.io picks up the connection details from browser cookies. You just need to sign into dropbox on the browser and webmethods.io does everything behind the scene![dropboxconnection](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/dropboxconnection.PNG)
![DropboxConnection_Success](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/dropboxconnectionsuccess.PNG)

5. Now map the source file to download from dropbox.![SourcefileMapping](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/sourcefilemapping.PNG)

6.  We have a cool feature which is sending email where you can send the content to respective audience. Search for "send an email" and drag and drop the "Send an Email" service to canvas.![AddSendEmail](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/addsendemail.PNG)

7.  Map the required fields in the Send an Email service. In the below example we have mapped the to address, subject and body![SendEmailMapping](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/sendemailmapping.PNG)

8. This completes the workflow and connects to stop step. We can test this from the UI to review the results in action tab. ![testingui](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/testingui.PNG)

9. Check the email to review the results of the workflow![Testing](https://github.com/maam1/webmethodsio-examples/blob/master/dropbox-sendemail/testing.PNG)
