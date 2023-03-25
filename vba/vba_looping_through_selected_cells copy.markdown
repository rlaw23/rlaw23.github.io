---
layout: page
title: Looping Through Selected Cells
parent: Excel VBA Automation
nav_order: 5
---

## Looping Through Selected Cells

<br/>

This is useful if, e.g. you want to send emails to certain customers in your long contact list, you can just select those several customers you need and run the snippet. Also see the section on how to [send emails](/vba/vba_send_email.html).


The Sub() repeatedly calls the demo_fn() in a loop and throws the current cell into the function:

{% highlight ruby %}
Sub Loop_Selected_Cells()

        For Each selected_cell In Selection
            Call demo_fn(selected_cell)
        Next selected_cell
    
End Sub
{% endhighlight %}

This function gets called repeatedly. It only prints row number of the current cell in the immediate window, but you can do what you need here:
{% highlight ruby %}
Function demo_fn(selected_cell)

    debug.Print selected_cell.Row

End Function
{% endhighlight %}
