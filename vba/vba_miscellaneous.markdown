---
layout: page
title: Miscellaneous
parent: Excel VBA Automation
nav_order: 8
---

## Miscellaneous

<br/>

Some miscellaneous VBA utility functions.

<br />
### 1. Add comment to a cell:
<br />
{% highlight ruby %}
Sub add_comment()

    Dim cmt As Comment
    Set cmt = ActiveCell.Comment
    If cmt Is Nothing Then
        ActiveCell.AddComment Text:=""
    End If

End Sub
{% endhighlight %}

<br />  
### 2. Wait for 2 seconds:
<br />

{% highlight ruby %}
Sub add_comment()
        
    Application.Wait (Now + TimeValue("0:00:02"))

End Sub
{% endhighlight %}

<br />
### 3. Send keys to simulate keyboard strokes:
<br />

{% highlight ruby %}
Sub add_comment()   

    Call SendKeys("abc~", True)

End Sub
{% endhighlight %}

<br />
### 4. Open an application that requires login and input username and ID:
<br />

{% highlight ruby %}
Sub open_app_with_login()   

    Call Shell(Range("application_path"), vbNormalFocus)
    Aplication.Wait (Now + TimeValue("0:00:10"))
    Call SendKeys("username{TAB}password~", True)
   
End Sub
{% endhighlight %}
