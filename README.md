# Syntax Coloring for AsciiDoc in BBEdit

## Introduction

This is a BBEdit Codeless Language Module that provides good highlighting for asciidoc files with a  in BBEdit (or the more basic, but free, TextWrangler). 

We are using this Language Module with BBEdit at [ProjectWizards](https://www.projectwizards.net) to write the documentation for [Merlin Project](https://www.projectwizards.net/en/merlin-project). Here you can see one example: https://www.projectwizards.net/en/support/documentation/merlin-project/handbook

## Installation

Copy AsciiDoc.plist into ~/Library/Application Support/BBEdit/Language Modules/. If no such folder exists, you may create it.


## Testing with Marked (version 2)

I have written this AppleScript snippet to display the current window of BBEdit in Marked 2 and copied the script to ~/Library/Application Support/BBEdit/Scripts/. If no such folder exists, you may create it.

	try
		tell application "BBEdit"
			set myFile to get file of front document of window 1
		end tell
	
		tell application "Marked 2"
			activate (open myFile)
		end tell
	end try
	
	
## Links

- BBEdit: http://www.barebones.com/products/bbedit/
- AsciiDoc(tor): http://asciidoctor.org/ (as the successor project to AsciiDoc)
- Marked: http://marked2app.com/
	
	
## License

Open source under the MIT License:

Copyright (c) 2013 ProjectWizards GmbH

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


## Contributors

Frank Blome ([@fblome](https://twitter.com/fblome))
