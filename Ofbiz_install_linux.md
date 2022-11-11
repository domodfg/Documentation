## Linux Installation

To Install Java (openjdk version 1.8.0.352)
```
sudo apt-get install openjdk-8-jdk
```
Switch to Java version (openjdk version 1.8.0.352)
```
sudo update-alternatives --config java
```
Check Java version
```
java -version
```
To Install Git
```
sudo apt install git
```
To clone the repo
```
git clone https://gitbox.apache.org/repos/asf/ofbiz-framework.git ofbiz-framework
```
Change directory into ofbiz
```
cd ofbiz-framework
```
```
git fetch --all --tags
```
```
git checkout release18.12.04
```
To build the program
```
./gradlew cleanAll loadAll
```
To run the program
```
./gradlew ofbiz 
```
To log into OFBiz, navigate with your browser to https://localhost:8443/accounting and login with username "admin" and password "ofbiz"
