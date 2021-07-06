# Law project
Project by Yuval Komash and Efrat Eitani
<br>
Using YAP-WRAPPER from https://github.com/amit-shkolnik/YAP-Wrapper

### Compiling and running YAP 
 
<b>Quick Start<b>
YAP has been tested and verified to run on Windows, Linux and MacOS.

Windows users: YAP doesn't handle Windows style text files that have BOM marks and CRLF newlines. So if you're running on Windows and YAP doesn't work make sure you don't have CRLF line endings and no BOM mark.

Requirements
<br>
Go
<br>
Git
<br>
bzip2
<br>
6GB RAM
<br>

Compilation
<br>
The following instructions are for Linux but similarly this can be done on Windows and MacOS.
<br>
Make sure you have Go and Git installed and on the command PATH.
<br>
<br>
Setup a Go environment:
<br>
Create a directory (usually per workspace/project) 
<br>
```$ mkdir yapproj; cd yapproj```
<br>
Set $GOPATH environment variable to your workspace:
<br>
```export GOPATH=path/to/yapproj```
<br>
in Windows use:
<br>
```set GOPATH=path/to/yapproj```
<br>
In the workspace directory create the src subdirectory:
 <br>
 ```mkdir src```
 <br>
cd into the src directory:
<br>
```cd src```
<br>
Clone the repository in the src folder of the workspace
 <br>
 ```git clone https://github.com/OnlpLab/yap.git```

Unzip the models and build the application:
```
$ cd yap
$ bunzip2 data/*.bz2
$ go get .
$ go build .
$ ./yap
./yap - invoke yap as a standalone app or as an api server
if ./yap is not working use yap.exe api
```
for more information about YAP:
https://github.com/OnlpLab/yap?fbclid=IwAR2BILOpxFyF051OaA-NkOXUDrgpCBzktEp-3I_UXzRCV2Hp2Eaf7JAsZJI#running-yap-as-a-restful-service
### Build and run application
Build the image manually by cloning the Git repo.
```
$ git clone https://github.com/eitanief/lawsProject.git
```
Inside "lawsProject" folder run:
```
pip install -r requirements.txt
```
```
$ python main.py
```

Open local host:

```
$ http://127.0.0.1:5000/
```





