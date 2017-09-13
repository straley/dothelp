Welcome to *dotHelp*.

If you want to see the normal bash help, use:

```
$ help help [options]
```

*dotHelp* will execute a ``.help`` bash script in  the current directory, if one exists.  If not, it'll try
to display a ``.help.txt`` file from the current directory.  And, if that does not exist, then it'll just
display this file.

If you don't want to put your help files in a directory (perhaps it is a GitHub project), then you can put
them in your home folder (or designated ``$DOTHELP`` path) with the relative path to that directory, with slashes
replaced with dashes, prepended with ``.help~``.

For instance, if you had a folder at ``~/Projects/backend/database/``, then the alternate help shell script would be:

``.help~Projects-backend-database``

Or the text file would be:

``.help~Projects-backend-database.txt``

If you want to add additional help files you can create files with a dash, like:
``.help-colors`` or ``.help-colors.txt``.  These will work like their undashed
counterparts, but will be displayed with:

```
$ help colors
```

Try ``help colors`` and learn about how to put colors in your help files.

You can place your *dotHelp* files in your home directory or specify a ``$DOTHELP`` path for them.
