#About
Adding .nanorc files as I find them here. This check-in contains .nanorc files from here: <http://code.google.com/p/nanosyntax/>, mostly.

#My Setup:

-		mkdir ~/.nano
-		git clone git://github.com/mattpowell/.nanorc.git ~/.nano
-		for f in ~/.nano/*.nanorc; do [ "$(grep ${f//$(echo ~)\/.nano\//} ~/.nanorc)" = '' ]&&(echo "include \"$f\"">>~/.nanorc)&&(echo "added $f to ~/.nanorc"); done

And that's it :). Third command will loop through all .nanorc files, replace ~ in file path, check if entry exists in .nanorc already, if not then add it.


#CHANGES

-	Commented out offending lines from this set of errors (diff of changes: <https://github.com/mattpowell/.nanorc/commit/e9a66f6db717e3befd950a0abe924262a8907307>):

		Error in /Users/mpowell/.nano/aptsrclist.nanorc on line 5: Bad regex "^deb(-src)? ((http|file|ftp):/[^ ]+|cdrom:\[[^\]]+\]/|cdrom:\[[a-zA-Z0-9\._-\(\) ]+\]/) [^ ]+ .+$": invalid character range

		Error in /Users/mpowell/.nano/aptsrclist.nanorc on line 7: Bad regex "^deb(-src)? ((http|file|ftp):/[^ ]+|cdrom:\[[^\]]+\]/|cdrom:\[[a-zA-Z0-9\._-\(\) ]+\]/) [^ ]+": invalid character range

		Error in /Users/mpowell/.nano/aptsrclist.nanorc on line 12: Bad regex "cdrom:\[[a-zA-Z0-9\._-\(\) ]+\]/": invalid character range

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/bash.nanorc on line 25: Bad regex "\<(aclocal|aconnect|aplay|apm|apmsleep|apropos|ar|arecord|as|as86|autoconf|autoheader|automake|awk|basename|bc|bison|c++|cal|cat|cc|cdda2wav|cdparanoia|cdrdao|cd-read|cdrecord|chfn|chgrp|chmod|chown|chroot|chsh|clear|cmp|co|col|comm|cp|cpio|cpp|cut|dc|dd|df|diff|diff3|dir|dircolors|directomatic|dirname|du|env|expr|fbset|file|find|flex|flex++|fmt|free|ftp|funzip|fuser|g++|gawk|gc|gcc|gdb|getent|getopt|gettext|gettextize|gimp|gimp-remote|gimptool|gmake|gs|head|hexdump|id|install|join|kill|killall|ld|ld86|ldd|less|lex|ln|locate|lockfile|logname|lp|lpr|ls|lynx|m4|make|man|mkdir|mknod|msgfmt|mv|namei|nasm|nawk|nice|nl|nm|nm86|nmap|nohup|nop|od|passwd|patch|pcregrep|pcretest|perl|perror|pidof|pr|printf|procmail|prune|ps2ascii|ps2epsi|ps2frag|ps2pdf|ps2ps|psbook|psmerge|psnup|psresize|psselect|pstops|rcs|rev|rm|scp|sed|seq|setterm|shred|size|size86|skill|slogin|snice|sort|sox|split|ssh|ssh-add|ssh-agent|ssh-keygen|ssh-keyscan|stat|strings|strip|sudo|suidperl|sum|tac|tail|tee|test|tr|uniq|unlink|unzip|updatedb|updmap|uptime|users|vmstat|w|wc|wget|whatis|whereis|which|who|whoami|write|xargs|yacc|yes|zip|zsoelim)\>": repetition-operator operand invalid

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/changelogs.nanorc on line 11: Bad regex "\<(CEST|CET|CST||CDT|EDT)\>": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/config.nanorc on line 2: Bad regex "(\.|/|)config$": empty (sub)expression

		Error in /Users/mpowell/.nano/config.nanorc on line 2: Bad regex "(\.|/|)logout$": empty (sub)expression

		Error in /Users/mpowell/.nano/config.nanorc on line 2: Bad regex "(\.|/|)COLORS$": empty (sub)expression

		Error in /Users/mpowell/.nano/config.nanorc on line 2: Bad regex "(\.|/|)colors$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/config2.nanorc on line 2: Bad regex "(\.|/|)env$": empty (sub)expression

		Error in /Users/mpowell/.nano/config2.nanorc on line 2: Bad regex "(\.|/|)server.$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/configfiles.nanorc on line 2: Bad regex "(\.|/|)conf$": empty (sub)expression

		Error in /Users/mpowell/.nano/configfiles.nanorc on line 2: Bad regex "(\.|/|)ample$": empty (sub)expression

		Error in /Users/mpowell/.nano/configfiles.nanorc on line 2: Bad regex "(\.|/|)globals$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/desc.nanorc on line 2: Bad regex "(\.|/|)desc$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/ebuild.nanorc on line 19: Bad regex "\<(do|new)(ins|s?bin|doc|lib(|\.so|\.a)|man|info|exe)\>": empty (sub)expression

		Error in /Users/mpowell/.nano/ebuild.nanorc on line 21: Bad regex "prepall(|docs|info|man|strip)": empty (sub)expression

		Error in /Users/mpowell/.nano/ebuild.nanorc on line 22: Bad regex "\<(|doc|ins|exe)into\>": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/ekghistory.nanorc on line 1: Bad regex "(\.|/|).gg/history": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/etc-stuff.nanorc on line 12: Bad regex "modules.d/(\.|/|)": empty (sub)expression

		Error in /Users/mpowell/.nano/etc-stuff.nanorc on line 165: Bad regex "/etc/ppp/peers/(\.|/|)": empty (sub)expression

		Error in /Users/mpowell/.nano/etc-stuff.nanorc on line 201: Bad regex "sane.d/(\.|/|)": empty (sub)expression

		Error in /Users/mpowell/.nano/etc-stuff.nanorc on line 223: Bad regex "(cdrom|cdrw|dvd|dvdrw|isdn|pty|vcs|vcsa|ippp|dcbri|ircomm|capi|card|nvidia|rtc|agpgart|psaux|ptmx|sd|dasd|)": empty (sub)expression

		Error in /Users/mpowell/.nano/etc-stuff.nanorc on line 276: Bad regex "xinetd.d/(\.|/|)": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/etcportage.nanorc on line 1: Command "Code:" not understood

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/etcxml.nanorc on line 12: Bad regex "/etc/fonts/(\.|/|)": empty (sub)expression

		Error in /Users/mpowell/.nano/etcxml.nanorc on line 12: Bad regex "/etc/xdg/(\.|/|)": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/gentoo.nanorc on line 19: Bad regex "\<(do|new)(ins|s?bin|doc|lib(|\.so|\.a)|man|info|exe|initd|confd|envd|pam|menu|icon)\>": empty (sub)expression

		Error in /Users/mpowell/.nano/gentoo.nanorc on line 21: Bad regex "prepall(|docs|info|man|strip)": empty (sub)expression

		Error in /Users/mpowell/.nano/gentoo.nanorc on line 22: Bad regex "\<(|doc|ins|exe)into\>": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/initscript.nanorc on line 3: Bad regex "/etc/init.d/(\.|/|)": empty (sub)expression

		Error in /Users/mpowell/.nano/initscript.nanorc on line 19: Bad regex "\<(do|new)(ins|s?bin|doc|lib(|\.so|\.a)|man|info|exe|initd|confd|envd|pam|menu|icon)\>": empty (sub)expression

		Error in /Users/mpowell/.nano/initscript.nanorc on line 21: Bad regex "prepall(|docs|info|man|strip)": empty (sub)expression

		Error in /Users/mpowell/.nano/initscript.nanorc on line 22: Bad regex "\<(|doc|ins|exe)into\>": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/maincf.nanorc on line 2: Bad regex "(\.|/|)cf$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/mcchangelog.nanorc on line 11: Bad regex "\<(CEST|CET|CST||CDT|EDT)\>": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/others.nanorc on line 109: Bad regex "/usr/bin(/|)|/usr/sbin|/bin|/sbin|/etc/init.d/": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/passwd.nanorc on line 2: Bad regex "(\.|/|)passwd$": empty (sub)expression

		Error in /Users/mpowell/.nano/passwd.nanorc on line 2: Bad regex "(\.|/|)shadow$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/postgresql.nanorc on line 2: Bad regex "\<(A(LL|NALY(S|Z)E|ND|NY|RRAY|S|SC|SYMMETRIC|UTHORIZATION)|B(ETWEEN|INARY|OTH|Y)|C(ASE|AST|HECK|OLLATE|OLUMN|ONSTRAINT|REATE|ROSS|URRENT_(DATE|ROLE|TIME|TIMESTAMP|USER))|D(EFAULT|EFERRABLE|ESC|ISTINCT|O|ROP)|E(LSE|ND|XCEPT)|F(ALSE|OR(EIGN)?|REEZE|ROM|ULL)|GRANT|GROUP|HAVING|I(LIKE|N(ITIALLY|NER|TERSECT|TO)?|S|SNULL)|JOIN|L(EADING|EFT|IKE|IMIT|OCALTIME(STAMP)?)|N(ATURAL|EW|OT(NULL)?|ULL)|O(FF(SET)?|LD|N|NLY|R|RDER|UTER|VERLAPS)|PLACING|PRIMARY|REFERENCES|RIGHT|S(ELECT|ESSION_USER|IMILAR|OME|YMMETRIC)|T(ABLE|HEN|O|RAILING|RUE)|UNION|UNIQUE|USER|USING|VE(IW|RBOSE)|WHEN|WHERE|)\>": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/privoxy.nanorc on line 1: Bad regex "(\.|/|)privoxy/config$": empty (sub)expression

		Error in /Users/mpowell/.nano/privoxy.nanorc on line 17: Bad regex "(\.|/|).action$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/profile.nanorc on line 2: Bad regex "(\.|/|)profile$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/rcfiles.nanorc on line 2: Bad regex "(\.|/|)control$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/sources_list.nanorc on line 6: Bad regex "^deb(-src)? ((http|file|ftp):/[^ ]+|cdrom:\[[^\]]+\]/|cdrom:\[[a-zA-Z0-9\._-\(\) ]+\]/) [^ ]+ .+$": invalid character range

		Error in /Users/mpowell/.nano/sources_list.nanorc on line 8: Bad regex "^deb(-src)? ((http|file|ftp):/[^ ]+|cdrom:\[[^\]]+\]/|cdrom:\[[a-zA-Z0-9\._-\(\) ]+\]/) [^ ]+": invalid character range

		Error in /Users/mpowell/.nano/sources_list.nanorc on line 13: Bad regex "cdrom:\[[a-zA-Z0-9\._-\(\) ]+\]/": invalid character range

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/tab.nanorc on line 2: Bad regex "(\.|/|)tab$": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/tcl.nanorc on line 16: Bad regex "^([[:space:]]+|)#.*": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/vhost.nanorc on line 4: Bad regex "(\.|/|)vhost\.conf": empty (sub)expression

		Press Enter to continue starting nano.


		Error in /Users/mpowell/.nano/xdefaults.nanorc on line 2: Bad regex "(\.|/|)default.$": empty (sub)expression

		Error in /Users/mpowell/.nano/xdefaults.nanorc on line 2: Bad regex "(\.|/|)resource.$": empty (sub)expression

		Press Enter to continue starting nano.


