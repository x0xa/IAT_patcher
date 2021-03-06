IAT patcher 
==========
Persistent IAT hooking application.<br/>
Read more: http://hasherezade.github.io/IAT_patcher/<br/>

Please report any bugs and remarks to: hasherezade@gmail.com<br/>

Requires:
+ bearparser: https://github.com/hasherezade/bearparser<br/>
+ Qt SDK (qt-sdk)<br/>
+ Qt4 Core (libqt4-core)<br/>
+ Qt4 GUI (libqt4-gui)<br/>
+ cmake http://www.cmake.org/<br/>

<h2>Autobuild:</h2></br>

To build it on Linux or MacOS you can use the given script - it automatically downloads this repository and all the dependencies:<br/>
https://github.com/hasherezade/IAT_patcher/blob/master/iatp_autobuild.sh<br/>
Just run it and it will do everything for you!

<h2>Manual build:</h2></br>

To have more control on the process of building, you can also build IAT Patcher manualy, by following several simple steps:<br/>
<b>1) Fetch sources:</b><br/>
<pre>
git clone https://github.com/hasherezade/IAT_patcher.git
cd IAT_patcher
git clone https://github.com/hasherezade/bearparser.git
</pre>

<b>2) Build (Linux example):</b><br/>
_NOTE: The same source should compile on Windows without problems, only generator (cmake -G ...) will be different_<br/><br/>
If you are in directory IAT_patcher, go up:
<pre>
cd ../
</pre>
and then:
<pre>
mkdir build
cd build
cmake -G [enviroment of your choice] ../IAT_patcher/
i. e
cmake -G "CodeBlocks - Unix Makefiles" ../IAT_patcher/
make
</pre>
...the application is here:
<pre>
../build/patcher/IAT_Patcher
</pre>
Videotutorial:
[![asciicast](https://asciinema.org/a/aakifgbiomqqnl0q08fzy3a62.png)](https://asciinema.org/a/aakifgbiomqqnl0q08fzy3a62)
