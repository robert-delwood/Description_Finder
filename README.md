# Description_Finder
A tool for extracting field descriptions from an OpenAPI file.

Description_Finder extracts all field descriptions from an OpenAPI file.
I was having trouble spellchecking and running linting tools on an entire OpenAPI file.
There can be a lot of intentional misspelling, such as field names.
For a large project, there can get into a signiicant number.
For linting, a similar situation happens.
There is a lot of text I don't want linted.
Writing specific linting rules to find those instances was complication, and in some cases, not possible.

Description_Finder extracts all field descriptions and copies them to the clipboard.
You can then paste, for example, into a text or word document.
You can use your favorite grammer tools at that point.
I typically use Word, taking advantage of it's spelling and grammar checks.
I can also use linters such as Vale much more conventiently. 
You will need to go back to the source file for changes.
After saving the changes Description_Finder can run again to get the descriptions listings.

Description_Finder is offered and used as it.
While I did test it, you may find limitations and problems.
Feel free to report any comments, questions, and converns, including bugs, to me.
I will look into them.
