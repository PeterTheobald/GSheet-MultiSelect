# GSheet-MultiSelect
Script to add Google Sheets MultiSelect fields from dropdown selections.

gsheets-multiselect - Google Sheets MultiSelect - @ControlAltPete 2023

Allow cells with data-validation to have multi-select.
The cell should have data validation from a range and 
the cell immediately above that validation range must contain:
MultiSelect:ShowInCell or MultiSelect:ShowRight or MultiSelect:ShowBelow

The default item separator is "value1, value2" but this can be changed
by adding ",Sep=" to the MultiSelect cell, eg: MultiSelect:ShowInCell,Sep=|
If the Sep has a comma or spaces you need quotes, eg: MultiSelect:ShowInCell,Sep=" , "

The special values '' (blank) 'None' and 'All' will replace all previously selected values.

Google Sheets will show a warning triangle when multiple items are selected,
This warning shows for ShowInCell but not for ShowRight or ShowBelow.
To hide this warning, add ",HideWarning" to the MultiSelect cell, eg: "MultiSelect:ShowInCell,HideWarning"
but be aware this will add a new dropdown option with all the current selected items
ie: the dropdown: 'Apple' 'Banana' 'Cherry' can become 'Apple' 'Banana' 'Cherry' 'Apple,Banana'
A limitation of HideWarning is it can only hide the warning for ONE input cell
If multiple input cells share the same data validation range and have different multi-select choices
only one of them will have the warning triangle hidden at a time.

Installation: Google Sheet, click on Extensions > Apps Script, paste this

![demo image1](demo-image1.png?raw=true "Demo image1")
![demo image2](demo-image2.png?raw=true "Demo image2")
![demo image3](demo-image3.png?raw=true "Demo image3")
