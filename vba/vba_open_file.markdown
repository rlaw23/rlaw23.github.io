---
layout: page
title: Opening a File
parent: Excel VBA Automation
nav_order: 2
---

## Opening a File

<br/>

Follow these steps to automate the process of opening a daily-generated system file:

1. Create an Excel formula to represent the daily file path:

    e.g. the full file path is "C:\Downloads\system_file_20230316.csv"
    
    Use the following formula: `="C:\Downloads\system_file_" & TEXT(TODAY(), "yyyymmdd") & ".csv"`

2. Name this cell as "file_path".

3. Create a VBA macro using the following code and assign to a button:



{% highlight ruby %}
Sub Open_Files()

    On Error GoTo ErrorHandler

    Set path = Range("file_path")
    
    Workbooks.Open path

    Exit Sub

    ErrorHandler:
        MsgBox "Error: File not found or cannot be opened."
        Exit Sub
    
End Sub
{% endhighlight %}
