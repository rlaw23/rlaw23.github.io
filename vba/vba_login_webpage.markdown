---
layout: page
title: Logging in a Webpage
parent: Excel VBA Automation
nav_order: 7
---

## Logging in a Webpage

<br/>

This code spins up Internet Explorer and fills in your credentials and login:

1. Name the cell that houses the signin page path as "webpage_path"
2. Create a VBA macro using the following code
3. Find out the relevant _element ID_, _class name_ and _tag name_ of the required fields in your target webpage so as to update the code below. You would need some basic knowledge about the HTML DOM.

{% highlight ruby %}
Sub IE_Webpage_Login()

    Dim IE As Object
    Set IE = CreateObject("InternetExplorer.Application")
    
    With IE
        .Visible = True
        .Navigate Range("webpage_path")
    
        Do Until .ReadyState = 4: DoEvents: Loop
    
        With .Document
            .getElementById("userId").Value = "username"
            .getElementById("password").Value = "password"
            .submit
        End With
    
        Do Until .ReadyState = 4: DoEvents: Loop
        Do While .Busy: DoEvents: Loop
    
    End With    
    
    Set IE = Nothing


End Sub
{% endhighlight %}


If `.submit` doesn't work, replace it with something like the below:

{% highlight ruby %}
            .getElementsbyclassname("button")(0).getElementsByTagName("a")(0).Click
{% endhighlight %}