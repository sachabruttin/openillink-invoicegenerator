# OpenILLink Invoice Generator

OpenILLink Invoice Generator is a Console Application generating MS Excel files (xlsx) from export file generated by [OpenILLink](https://github.com/openillink-project/openillink). 

It specifically target the [OpenILLink UNIGE instance](https://bibliotool.unige.ch/openillink/index.php).

## Requirements

.NET Framework 4.6

## Run it

From the command line (e.:

```cmd
 > openillink.invoicegenerator.exe --help
```

## Parameters

|short|long|required|description|default
|---|---|---|---|---|---
|-i | --input | true | Input file to be processed.|
|   | --from  | false| From date (format yyyy-mm-dd)|0001-01-01
|   |  --to   | false| To date (format yyyy-mm-dd)|Today

## Quick Start Examples

Generate for all orders in the file:

```cmd
 > openillink.invoicegenerator.exe -i openillink.csv
```

Generate for orders from 1st of January 2017 to today:

```cmd
 > openillink.invoicegenerator.exe -i openillink.csv --from 2017-01-01
```

Generate for orders until 31 december 2017:

```cmd
 > openillink.invoicegenerator.exe -i openillink.csv --to 2017-12-31
```


Generate for orders from 1st of January 2017 to 31 of December 2017:

```
 > openillink.invoicegenerator.exe -i openillink.csv --from 2017-01-01 --to 2017-12-31
```