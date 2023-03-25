---
layout: page
title: Sending Emails
parent: Excel VBA Automation
nav_order: 6
---

## Sending Emails

<br/>

If you have to send some standardized emails daily, you are probably "replying all" to yesterday's email and painfully manually editing subjects and contents every day. Try the below instead.

If you are looking for something more capable than mail merge, you will also find this to be helpful.

This code requires early binding. Please check `Tools > Reference > "MICROSOFT OUTLOOK 14.0 OBJECT LIBRARY"`

Change the recipients, subjects, contents and attachment links below to your needs.

{% highlight ruby %}
Sub send_email()
    
        
    Dim OutlookApp As Outlook.Application
    Dim OutlookMail As Outlook.MailItem
    
    Set OutlookApp = New Outlook.Application
    Set OutlookMail = OutlookApp.CreateItem(olMailItem)
    
    Set mainsheet = Sheets("Sheet1")
    set attachment_link = "C:\Downloads\attachment.pdf"
    
    
    With OutlookMail
        .BodyFormat = olFormatHTML
        .Display
        .HTMLBody = "<span>Email content in html.</span>" & .HTMLBody
        .To = "recipient1@mail.com"
        .CC = "recipient2@mail.com"
        '.BCC = "recipient3@mail.com"
        Subject = "Email subject " & Format(Date, "dmmmyyyy")
        '.Attachments = ThisWorkbook
        '.Attachments.Add attachment_link
        '.Send
    

End Sub
{% endhighlight %}
