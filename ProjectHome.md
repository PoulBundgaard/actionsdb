This is a simple program written with freepascal in Lazarus. The core of it is the Sqlite3 database todo.db. The program helps to manipulate on the records which contain information on the actions a user wants to be done.

The compilation is tested on Windows XP and Linux (Gentoo).

To compile the program, it is assumed that the following programs are installed:
<pre>
Lazarus (>= 0.9.26)<br>
fpc (>=2.2.2)<br>
sqlite 3 (>=3.6.6.2)<br>
</pre>
Additionally, Sqlite3Dataset component should be installed in Lazarus.

Files:
<pre>
README    	README<br>
COPYING         License<br>
todo.db         SQLite3 database<br>
dump.txt        SQLite3 database dump to generate db in case of need<br>
todo.sh         Bash script to work with db from cli<br>
</pre>

Lazarus files:
<pre>
actions.lpi<br>
actions.lpr<br>
unit1.lfm<br>
unit.pas<br>
etc.<br>
</pre>

HOW TO USE

Just open actions.lpr in Lazarus and compile the code.

When the compilation is done, make sure that the compiled binary, todo.db, (and optionally sqlite3.dll) are in one directory. Execute the binary to work.

The generated binary file can be smaller in size in you use strip and upx utilities on them.

If you have questions , mail me record200ATgmail.com