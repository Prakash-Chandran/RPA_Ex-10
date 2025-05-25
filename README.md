# RPA_Ex-10

# Exercise-10-Email-Automation---send-email

~~~
Name : PRAKASH.C  
Reg.No : 212223240122  
~~~

## Aim
To create a UiPath workflow that sends an email using a Gmail account through SMTP or Outlook activities.

## Materials Required

UiPath Studio
Gmail account
Internet connection
Mail Activities package (installed by default)
Enable "Less secure apps access" or App Passwords in Gmail settings (if 2FA is enabled)

## Procedure

### Step 1: Setup Gmail for SMTP Access
Enable 2-Step Verification on your Gmail account.
Go to https://myaccount.google.com/apppasswords
Generate an App Password (e.g., for "Mail on Windows Computer"). 
Copy and save the app password securely — you’ll use it in UiPath.

### Step 2: Create a New UiPath Process
Open UiPath Studio and create a new process named GmailSenderBot.

### Step 3: Use Send SMTP Mail Message
Drag the Send SMTP Mail Message activity (found in UiPath.Mail.SMTP.Activities).

Fill in the properties:

Property	Value
To	"recipient@example.com"
Subject	"Test Email from UiPath"
Body	"Hello! This is a test email from UiPath automation."
Port	587
Server	"smtp.gmail.com"
Email	"your_email@gmail.com"
Password	Paste your Gmail App Password securely
SecureConnection	StartTls

### Step 4: Run the Workflow
Save and run the bot.

The email will be sent to the recipient from your Gmail account.

## OUTPUT:
An email will be delivered to the recipient with the subject and message body specified.

![10-1](https://github.com/user-attachments/assets/dd5ed696-cd23-45e3-bb72-205c5c79019c)

![10-2](https://github.com/user-attachments/assets/3b0f9db6-2339-4edf-a7d0-451699d7db29)

![10-3](https://github.com/user-attachments/assets/cfa7a9be-e56d-4bda-86e0-32c99c0cd447)


## Result:
The UiPath workflow successfully sends an email from a Gmail account using SMTP configuration.
