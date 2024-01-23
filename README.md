# Help!

The `helprc` file provides some functions which can print some useful help information to the console.  These are a limited set of useful commands which can be used as an aide memoir or for copy paste while working in the console.

## Gettings started

Source the `helprc` file from your `.bashrc` or `.zshrc` file:
```
source ~/help/helprc
```

Better yet: link this file within a folder, `EXTERNALRCS`, containing other rc file and load them all together:
```
EXTERNALRCS="~/rcs/"
for RCFILE in "$EXTERNALRCS"*
do
  if [ -f "$RCFILE" ]; then
    source $RCFILE
  fi
done
```
