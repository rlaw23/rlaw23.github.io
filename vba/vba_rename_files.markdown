---
layout: page
title: Renaming Files
parent: Excel VBA Automation
nav_order: 4
---

## Renaming Files

<br/>

Follow these steps to rename multiple files with VBA:

1. Input the original file names in Column A, starting from row 1.

2. Input the target file names in Column B, starting from row 1.

3. Input the folder path into a cell, e.g. `C:\Downloads\`, and name that cell "folder_path"

4. Create a VBA macro using the following code and assign to a button:



{% highlight ruby %}
Sub Rename_Files()

    With Sheets("Sheet1")
        For i = 1 to .Range("A1").End(xlDown).Row
            Name .Range("folder_path") & .Range("A" & i) & ".csv" As .Range("folder_path") & .Range("B" & i) & ".csv"
        Next i
    
    End With

End Sub
{% endhighlight %}
