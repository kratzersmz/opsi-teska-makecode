# opsi-teska-makecode
Place makecode Installation in makecode Dir on opsi Server. To get the makecode installation:

start new makecode downloaded from website(so it unpacks the installation)
go to %appdata%\Local\makecode_microbit\ and copy all files/folders to makecode directory on the opsi server
makecode opsi Dir should look like this
<pre>
\\OPSI-SERVER\opsi_depot_rw\teska-makecode\makecode

14.11.2019  12:51    <DIR>          .
14.11.2019  12:51    <DIR>          ..
14.11.2019  12:50    <DIR>          app-2.0.3
14.11.2019  12:51            15.086 app.ico
14.11.2019  12:50           295.760 MakeCode for microbit.exe
14.11.2019  12:50    <DIR>          packages
14.11.2019  12:51             1.699 SquirrelSetup.log
14.11.2019  12:50         1.876.760 Update.exe
               4 Datei(en),      2.189.305 Bytes
               4 Verzeichnis(se), 68.700.766.208 Bytes frei
  </pre>

# howto build
1. start a ssh session to your opsi server
2. change to /home/opsiproducts (if you use paedml linux + win =< 3.x)
3. type in git clone https://github.com/kratzersmz/opsi-teska-makecode.git
4. change to /home/opsiproducts/opsi-teska-makecode
5. type in opsi-makepackage -> your *.opsi package will be generated
6. install package with opsi-package-manager -i opsi-teska-makecode.opsi
7. refresh your opsi config editor

