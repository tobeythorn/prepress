Prepress.py
===========


Introduction
------------

Prepress.py is a simple static site generator written in Python.

* Supports Prepress plain text format
* Supports front matter
* Supports root-relative links via //



Build and test a default site
-----------------------------

Download and unzip Prepress.py. Open Terminal. Change directory to “prepress”. To build your site, run the following command:

	python3 prepress.py

In another Terminal window, change directory to “site” and run:

	python3 -m http.server

To test your site, open your browser and go to:

	localhost:8000



Edit your site
--------------

The Prepress directory structure is shown below.

	prepress
		└── pages
		└── components
		└── layouts
		└── site
			└── static
				└── audio
				└── css
				└── image
				└── scripts
				└── video

Open index.pre in “pages”. Any plain text editor will do. Under “Introduction”, write a few words about your site. Save the file.

Now open masthead.pre in “components”. Change “My site” to the name you would like your site to have. You can change this later at any time. Save it.

In Terminal, rebuild your site:

	python3 prepress.py

And in your browser go to:

	localhost:8000

You should see the changes you just made.



Deploy your site to the web
---------------------------

To publish your site to the web, just upload the contents of your “site” directory to the root directory on your hosting service.

If your site will be hosted in a sub-directory, specify the base relative to the root when you build.

	python3 prepress.py /project_1/



Deploy your site to Github Pages
--------------------------------

Create an account on github.com, if you don't have one already. Create a repository called:

	username.github.io

Where “username” is your actual github username.

Drag and drop the contents of your “site” directory into your repository. Click commit.

To view your site, open a browser and go to:

	https://username.github.io/

Where “username” is your actual Github username. Note that you may need to wait a few minutes for Github to update changes to your site.



License
-------

	Copyright 2020-present, Tobey Thorn. All rights reserved.
	
	Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
	
	Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution. Neither the name “Protowrite” nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission. 
	
	THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.



Download
--------

[Prepress.py 0.9.0 (130KB)](https://github.com/tobeythorn/prepress.py/raw/main/prepress.zip)

