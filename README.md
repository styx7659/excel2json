excel2json
==========
excel2json is tool that generates JSON files from well-formed excel datas

## FEATURES
* Automatic search source excel files on directory located excel2json tool
* .json file generates per workbook's sheet (filename is same as sheet name)
 * Sheet name must be prefixed '!' mark (see example.xlsx)
 * Not prefixed sheet will be ignored
* Supports generating complex tree hierarchy JSON model
 * Object in Objects, Array in Objects, Objects in Array all of cases that JSON represents
 * N-depth hierarchy ( as you want to )
* Excel formula evaluatation supports

## HOW TO DEFINE JSON SCHEME IN XLS FILE 

## CONSTRAINTS
* Supports only version of Excel 2007 (or higher)
* excel2json Needs at least the Java Runtime Environment v1.8
* Source-code is not provide yet

## SIMILAR PROJECTS THAT I'VE FOUND ON GitHub
https://github.com/coolengineer/excel2json
https://github.com/mhaemmerle/excel-to-json

## COMMAND-LINE ARGUMENTS


## WARNING
1. Too many VLOOKUP formula use in excel data can cause poor performance 
2. Empty cell will be removed parent level of json hierarchy
3. Not supports all of formulas. To find which formula excel2json supports read this page first (https://poi.apache.org/spreadsheet/formula.html) because excel2json implements by Apache POI projects 