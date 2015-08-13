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
For this lesson, we will be running `express` right in this repo's directory.
We want it to use Handlebars for view rendering, since that's what we're
familiar with, so we use the `--hbs` flag. Finally, we specify `.` for the
directory to create files in. It will ask us to confirm since this is a
non-empty directory.

```bash
$ express --hbs .
```

Now, having run that, take a look around at what `express` has generated
for us:

```bash
$ ls -l
```

You should see a directory listing that resembles this:

	-rw-rw-r-- 1 saad saad 1441 Aug 13 12:13 app.js
	drwxr-xr-x 2 saad saad 4096 Aug 13 12:13 bin
	-rw-rw-r-- 1 saad saad  339 Aug 13 12:13 package.json
	drwxr-xr-x 5 saad saad 4096 Aug 13 12:13 public
	-rw-rw-r-- 1 saad saad 1425 Aug 13 12:07 README.md
	drwxr-xr-x 2 saad saad 4096 Aug 13 12:13 routes
	drwxr-xr-x 2 saad saad 4096 Aug 13 12:13 views

##Files
###package.json
This is the `npm` package file for your application. It contains various
metadata, most importantly dependencies and development-only dependencies.
Have a look at its contents by opening it up in Sublime or by running the
following command:

```bash
$ less package.json
```








