---
layout: page
title: Opening a Folder
parent: Excel VBA Automation
nav_order: 1
---

## Opening a Folder

<br/>            
                
Follow these steps to automate the process of opening folder:

1. Create an Excel formula to represent the folder path:
    
    e.g. Use the following formula: `="C:\Downloads\`

2. Name this cell as "folder_path".

3. Create a VBA macro using the following code and assign to a button:



{% highlight ruby %}
Sub Open_Folder()

    Call Shell("explorer.exe" & " " & Range("destination_folder"), vbNormalFocus)

End Sub
{% endhighlight %}
