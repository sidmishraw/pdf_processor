## IEEE Xplore PDF - JSON converter

## Motivation and Objective
The PDF document source, unlike markup langauges is diffuclt to comprehend when read in using an application.
It is difficult to extract words from the PDF's source.
This utility tries to tackle this problem of extracting words from the PDF document's source and converting it
into a JSON.

The JSON is going to have the following structure:

```javascript
{
  "Page#1": [
    "Observational",
    "Calculi",
    "Classes",
    "of",
    "Association",
    "Rules",
    "and",
    "F-property"
    ]
}
```
`Page#1` represents the page of the PDF document and it's value is the list of words occuring in page 1 of the PDF document.

>Note: At the moment, this utility only focusses on the PDF documents found on IEEE's Xplore website.

>Note: This utility makes use of [`PDFMiner`](https://github.com/euske/pdfminer) utility made by `Yusuke Shinyama`.

### Min req: Python v3.5.2
