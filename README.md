COMPARING 2 UNORDERED XML DOCUMENTS USING XDIFF LIBRAIRY WITH NODEJS

#INSTALLATION

1) Compile java source of X-Diff librairy running "make.bat"
2) "npm run compare"
3) Adapt script.js to your needs

#XDIFF
			
			X-Diff	Version 0.9.6

What is it?
-----------

X-Diff is a tool for detecting difference between two XML documents.


Documentation
-------------

The core algorithm of X-Diff is described in the paper, "X-Diff: An
Efficient Change Detection Algorithm for XML Documents", ICDE 2003.
(http://www.cs.wisc.edu/~yuanwang/research/xdiff.pdf).


Installation
------------

-- Java version:

Required: Xerces Java v1.4.0+.

On UNIX/LINUX,

	tar zxf xdiff-j-0.9.6.tar.gz
	cd X-Diff
	make

On Windows,

	unzip xdiff-j-0.9.6.zip
	cd X-Diff
	make.bat

-- C++ version

Required: Xerces C++ v1.4.0, g++ v2.9.*

	tar zxf xdiff-j-0.9.6.tar.gz
	cd X-Diff
	make


Running X-Diff
--------------

java XDiff [-o|-g] [-p percent] xml_file1 xml_file2 result_file

or,

xdiff [-o|-g] [-p percent] xml_file1 xml_file2 result_file

Options:

	The default mode is "-o -p 0.3".
	
  -o	The optimal mode, to get the diff result with minimum editing
  	distance.
	
  -g	The greedy mode, to get a diff result quickly, the result may not
  	be "optimal".
	
  -p	The maximum change percentage allowed. X-Diff will not try to match
  	nodes that are much different from each other.


Bug Reporting
-------------

Please report any bugs or send your comments to Yuan Wang at
yuanwang@cs.wisc.edu


Copyright Information
---------------------

X-Diff is an open source product, which open source license permits you to
use X-Diff at no charge under the condition that if you use the software in
an application you redistribute, the complete source code for your application
must be available and freely redistributable under reasonable conditions.
If you do not want to release the source code for your application, you may
purchase a license from me.



Copyright (c) 2001 - 2005
	Yuan Wang. All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions
are met:
1. Redistributions of source code must retain the above copyright notice,
this list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright
notice, this list of conditions and the following disclaimer in the 
documentation and/or other materials provided with the distribution.
3. Redistributions in any form must be accompanied by information on
how to obtain complete source code for the X-Diff software and any
accompanying software that uses the X-Diff software.  The source code
must either be included in the distribution or be available for no 
more than the cost of distribution plus a nominal fee, and must be
freely redistributable under reasonable conditions.  For an executable
file, complete source code means the source code for all modules it
contains.  It does not include source code for modules or files that 
typically accompany the major components of the operating system on
which the executable file runs.

THIS SOFTWARE IS PROVIDED BY YUAN WANG "AS IS" AND ANY EXPRESS OR IMPLIED
WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF 
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR NON-INFRINGEMENT,
ARE DISCLAIMED.  IN NO EVENT SHALL YUAN WANG BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, 
STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING 
IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE 
POSSIBILITY OF SUCH DAMAGE.

