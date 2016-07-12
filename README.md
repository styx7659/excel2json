excel2json
==========
* Copyright (C) 2016 by WooJun Shim woojun.shim@gmail.com
* Korean description available in http://nvidian7.github.io
* excel2json is tool that generates JSON files from well-formed excel datas

## Purpose
* Determining how to represents game data is the biggest factor of development
 * Generally, designers wants to manage data in excel
 * Programmer wants to text-based, hierarchical structured data (e.g. JSON, XML) 
* excel2json can be easily generate JSON files from excel data 

## Features
* Automatic search source excel files on directory located excel2json tool
* .json file generates per workbook's sheet (filename is same as sheet name)
 * Sheet name must be prefixed '!' mark (see example.xlsx)
 * Not prefixed sheet will be ignored
* Supports generating complex tree hierarchy JSON model
 * Object in Objects, Array in Objects, Objects in Array all of cases that JSON represents
 * N-depth hierarchy ( as you want to )
* Excel formula evaluatation supports
* Using cell merge feature to represents Object or Array's scope

## How to define JSON scheme in xls files 

Please see sample.xlsx and commited json files :)
If you are familiar with JSON-structure will soon be able to understand


## Constraints
* Supports only version of Excel 2007 (or higher)
* excel2json Needs at least the Java Runtime Environment v1.8
* Source-code is not provide yet, sort of...

## Similar projects that I've found on GitHub
* https://github.com/coolengineer/excel2json
* https://github.com/mhaemmerle/excel-to-json

## Command line arguments


## Warning
1. Too many VLOOKUP formula use in excel data can cause poor performance 
2. Empty cell will be removed parent level of json hierarchy
3. Not supports all of formulas. To find which formula excel2json supports read this page first (https://poi.apache.org/spreadsheet/formula.html) because excel2json implements by Apache POI projects 