## Mac Installation

To Install Java (openjdk version 1.8.0.352)
```
brew install adoptopenjdk/openjdk/adoptopenjdk8
```
Switch Java version  to openjdk 1.8.0.352
```
export JAVA_HOME=`/usr/libexec/java_home -v 1.8`
```
Check Java version
```
java -version
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
./gradlew "ofbiz --load-data readers=seed,seed-initial" loadAdminUserLogin -PuserLoginId=admin
```
To run the program
```
./gradlew ofbiz 
```
To log into OFBiz, navigate with your browser to https://localhost:8443/accounting and login with username "admin" and password "ofbiz"

### Resources
- https://medium.com/@devkosal/switching-java-jdk-versions-on-macos-80bc868e686a
- https://dzone.com/articles/install-openjdk-versions-on-the-mac
