excel2json
==========
excel2json is tool which generates json format text file from formed-excel data

## FEATURES
* Generate JSON format file from well-formed excel data files
 * Automatic search source excel files on directory located excel2json tool
 * .json file generates per workbook's sheet (filename is same as sheet name)
  * Sheet name must be prefixed '!' mark (see example.xlsx)
  * Not prefixed sheet will be ignored
 * Supports generating complex tree hierarchy JSON model
 * Excel's formula supports

## WARNING
1. Too many VLOOKUP formula use in excel data can cause poor performance 
2. Empty cell will be removed parent level of json hierarchy
3. Not supports all of formulas. To find which formula excel2json supports read this page first (https://poi.apache.org/spreadsheet/formula.html) because excel2json implements by Apache POI projects 