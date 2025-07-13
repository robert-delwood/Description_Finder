# Description_Finder
A tool for extracting field descriptions from an OpenAPI file.

## Introduction
*Description_Finder* extracts all field descriptions from an OpenAPI file.
I was having trouble spellchecking and running linting tools on an entire OpenAPI file.
There can be a lot of intentional misspelling, such as field names.
For a large project, there can get into a significant number.
For linting, a similar situation happens.
There is a lot of text I don't want linted.
Writing specific linting rules to find those instances was complication, and in some cases, not possible.

*Description_Finder* extracts all field descriptions and copies them to the clipboard.
You can then paste, for example, into a text or word document.
You can use your favorite grammar tools at that point.
I typically use Word, taking advantage of its spelling and grammar checks.
I can also use linters such as Vale much more conveniently. 
You will need to go back to the source file for changes.
After saving the changes *Description_Finder* can run again to get the descriptions listings.

## Prerequisites
*Description_Finder* runs under Windows only.

## Downloading *Description_Finder*
To download *Description_Finder*,
1. Navigate to my GitHub repository, if you are not already there: https://github.com/robert-delwood/Description_Finder
1. Select the file: Description_Finder.exe
1. Select **Raw**. This displays an open file dialog.
1. Navigate to the download location of your choice.
1. Select **Save**. This saves the file to that location.

## Running Description_Finder
To run *Description_Finder*,
1. Double click the application Description_Finder.exe.
It opens to the *Description_Finder* window.

## Caveats
*Description_Finder* is offered and used as it.
While I did test it, you may find limitations and problems.
Feel free to report any comments, questions, and concerns, including bugs, to me.
I will look into them.
