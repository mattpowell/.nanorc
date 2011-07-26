#About
Adding .nanorc files as I find them here. This check-in contains .nanorc files from here: <http://code.google.com/p/nanosyntax/>, mostly.

#My Setup:

>	mkdir ~/.nano
>	git clone git://github.com/mattpowell/.nanorc.git ~/.nano
>	for f in ~/.nano/*.nanorc; do [ "$(grep ${f//$(echo ~)\/.nano\//} ~/.nanorc)" = '' ]&&(echo "include \"$f\"">>~/.nanorc)&&(echo "added $f to ~/.nanorc"); done

And that's it :). Third command will loop through all .nanorc files, replace ~ in file path, check if entry exists in .nanorc already, if not then add it.
