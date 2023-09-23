# GSheet-MultiSelect
Script to add Google Sheets MultiSelect fields

gsheets-multiselect - Google Sheets MultiSelect - @ControlAltPete 2023

Allow cells with data-validation to have multi-select
The cell should have data validation from a range and 
the cell immediately above that validation range must contain:
MultiSelect:ShowInCell or MultiSelect:ShowRight or MultiSelect:ShowBelow
The default values list display separator is "value1, value2" but
can be changed by adding ",Sep=" to the MultiSelect cell, eg: "MultiSelect:ShowInCell,Sep= | "
The special values '' (blank) 'none' and 'all' will replace all previously selected values.

Installation: Google Sheet, click on Extensions > Apps Script, paste the script
