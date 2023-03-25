---
layout: page
title: Copying a File
parent: Excel VBA Automation
nav_order: 3
---

## Copying a File

<br/>

Follow these steps to automate the process of copying a daily-generated system file:

1. Create an Excel formula to represent the file path of the source file:

    e.g. the full file path is "C:\Downloads\system_file_20230316.csv"
    
    Use the following formula: `="C:\Downloads\system_file_" & TEXT(TODAY(), "yyyymmdd") & ".csv"`

2. Name this cell as "source_filepath".

3. Create an Excel formula to represent the path of the destination folder:

    e.g. the full folder path is "C:\Destination_202303\"
    
    Use the following formula: `="C:\Destination_" & TEXT(TODAY(), "yyyymm")`

4. Name this cell as "destination_folder".

5. Create an Excel formula to represent the file path of the destination file:

    e.g. the full file path is "C:\Destination_202303\system_file_20230316.csv"
    
    Use the following formula: `="C:\Destination_" & TEXT(TODAY(), "yyyymm") & "\system_file_" & TEXT(TODAY(), "yyyymmdd") & ".csv"`

6. Name this cell as "destination_filepath".

7. Create a VBA macro using the following code and assign to a button:


{% highlight ruby %}
Sub Copy_Files()

    Dim fso As Object
    Set fso = VBA.CreateObject("Scripting.FileSystemObject")
    
    On Error Resume Next
    MkDir Range("destination_folder")
    
    Call fso.CopyFile(Range("source_filepath"), Range("destination_filepath"))
    
    Call Shell("explorer.exe" & " " & Range("destination_folder"), vbNormalFocus)

End Sub
{% endhighlight %}


This code snippet will create the destination folder if it doesn't already exist.