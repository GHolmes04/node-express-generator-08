#Express Generator

##What is it?
Express generator, known to `npm` as `express-generator`, is something that
will save you more time and typing than you can measure when starting an
express back-end.

##Install it
Like most node packages, we will be installing `express-generator` with `npm`.

Take note of the shell prompts. For Mac, you will be able to globally install
this package with your ordinary account. For Linux, you will need superuser
privileges. Prefix the command with `sudo` or otherwise assume a superuser
(`root`) role before running it.

###Mac OS X
```bash
$ npm install -g express-generator
```

###Linux
```bash
# npm install -g express-generator
```

###Verify install
Run this command to verify that `express-generator` has been successfully
installed:

```bash
$ express -h
```

If successful, you should see this output:

	Usage: express [options] [dir]

	Options:

		-h, --help          output usage information
		-V, --version       output the version number
		-e, --ejs           add ejs engine support (defaults to jade)
			--hbs           add handlebars engine support
		-H, --hogan         add hogan.js engine support
		-c, --css <engine>  add stylesheet <engine> support (less|stylus|compass|sass) (defaults to plain css)
			--git           add .gitignore
		-f, --force         force on non-empty directory

##Use it
For this lesson, we will be running `express` right in this directory.



