cuke-steps
==========

Cucumber step documentation.

This is a small script that reads Cucumber/Gherkin step definition files and outputs pretty-printed documentation of those steps.  It is meant as a tool for developers to easily see what step definitions already exist.

Currently supported output format is HTML. 

Usage
-----

> ruby cuke-steps.rb \[options\] &lt;directories...&gt;

In its simplest form:

> ruby cuke-steps.rb features/

Supported options:

*  -f FORMAT, --format FORMAT  
   Select output format, so far only "html"

*  -o FILE, --output FILE  
   Output to FILE, default "steps.html"

*  -h, --help  
   Usage instructions

This will scan the provided directories for step definition files (*.rb) and output the documentation in the specified file.

The tool supports having step definitions in multiple directories.  It will generate a separate section for each directory specified on the command line.


TODO
----

*  Add markdown export type
*  Create a gem out of it


---

BSD License
-----------

Copyright (c) 2012, Sampo Niskanen
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met: 

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer. 
2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution. 

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

