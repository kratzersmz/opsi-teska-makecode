# opsi-teska-makecode
Place makecode Installation in makecode Dir on opsi Server. To get the makecode installation:

start new makecode downloaded from website(so it unpacks the installation)
go to %appdata%\Local\makecode and copy alle files to makecode directory on the opsi server
makecode opsi Dir should look like this

# howto build
1. start a ssh session to your opsi server
2. change to /home/opsiproducts (if you use paedml linux + win =< 3.x)
3. type in git clone https://github.com/kratzersmz/opsi-teska-makecode.git
4. change to /home/opsiproducts/opsi-teska-makecode
5. type in opsi-makepackage -> your *.opsi package will be generated
6. install package with opsi-package-manager -i opsi-teska-makecode.opsi
7. refresh your opsi config editor
