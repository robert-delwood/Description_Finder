# Description_Finder
A tool for extracting field descriptions from an OpenAPI file.

## Introduction
*Description_Finder* extracts all field descriptions from an OpenAPI file.
I was having trouble spellchecking and running linting tools on an entire OpenAPI file.

For spell checks, there can be a lot of intentional misspelling, such as field names.
For a large project, this can get into a significant number.
For linting, a similar situation happens.
There is a lot of text I don't want linted, such as comments, summaries, and code examples.
Writing specific linting rules to find only those instances is complication, and in some cases, impossible.
Both of these cases make checking the file as a whole difficult.

*Description_Finder* extracts all field descriptions and copies them to the clipboard.
It copies only the text from a field description. 
These are defined as path, query, request, and response fields.
Fields can be nested deeply.
This application finds description tags inside any number of object nestings.
You can then paste, for example, into a text or Word document.
You can use your favorite grammar tools at that point.
I typically use Word, taking advantage of its spelling and grammar checks.
I can also use linters such as Vale, much more conveniently. 
You make changes to the source file,
After saving the changes, *Description_Finder* can run again to get the current descriptions listings.

## Prerequisites
* *Description_Finder* runs under Windows only.
The plans for a Mac version are uncertain.
* The OpenAPI file must be less than version 3.1.0. If this is a problem, in many cases, the OpenAPI files's version number can be changed to 3.0.3 safely.
* The OpenAPI file must be well-formed and conform to the OpenAPI specification.
* For best results I recommend using a fully deferenced OpenAPI file.
That is, a file with no $ref statements.
In most cases $ref statements are accurately handled but due to OpenAPI coding differences, I can't assure accurate reporting.

## Downloading *Description_Finder*
To download *Description_Finder*,
1. Navigate to my GitHub repository, if you are not already there: https://github.com/robert-delwood/Description_Finder
1. Select the file: Description_Finder.exe
1. Select **Raw**. This displays a save file dialog.
1. Navigate to the download location of your choice.
1. Select **Save**. This saves the file to that location.

## Running Description_Finder
To run *Description_Finder*,
1. Double click the application Description_Finder.exe.
It opens to the *Description_Finder* window.

## Operations
To get a list of descriptions:
1. Select **Open OpenAPI file**. This displays an open file dialog.
1. Navigate to, and then select the target OpenAPI source file.
1. Select **Open**. This opens the file and starts its processing. 
This may take a moment depending on the file size and internal complexity.

By default, the descriptions are automatically copied to the clipboard.
Without any additional involvement with the application, you can paste the clipboard into another document.
For example, this may be in Microsoft Word or as any text file.

The application shows the OpenAPI document's structure as tree view of all the paths. 
Any path may be expanded by clicking on it.
* Multiple clicks may be needed to fully traverse a branch.
* Clicking an open branch closes it.
* Multiple branches any be open at the same time.

The tree view provides no additional functionality other than being able to visually see the field structures with an endpoint.
You cannot get the descriptions for a specific branch of field.

## The Buttons

**Open OpenAPI file**. This selects and opens an OpenAPI source file. Once selected, the processing is automatic. This includes copying the descriptions to the clipboard. No additional action is required.

**Copy description to clipboard**. This copies the descriptions to the clipboard. This allows you to copy other items after first opening the application. The application is not re-run, nor is re-opening the source file required.

**Open all first levels**. This opens all first levels of each endpoint.

**Open all second levels**. This opens all second levels of each endpoint.

**Close all levels**. This closes all levels for each endpoint.

**Automatically copy to clipboard** (checkbox). This sets the default capability for automatically copying descriptions to the clipboard. There may instances when you want to see the field structures but not copy descriptions to the clipboard.<br>
* If checked, descriptions are copied to the clipboard.<br>
* If unchecked, descriptions are copied to the clipboard.

## Caveats
*Description_Finder* is offered and used as is.
While I did test it, you may find limitations and problems.
Feel free to report any comments, questions, and concerns, including bugs, to me.
I will look into them.
