## Windows Installation:
Install Java SE Development Kit 11.0.16.1 on https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html
<br>
Remove other versions of Java Jdk in control panel
<br>
Restart PC
<br>
Check The java version by typing in CMD, it should display 11.0.16.1
```
java -version
```
Install Git on https://git-scm.com/download/win
<br>
Launch Git Bash, 
Inside the bash terminal type:
```
cd Downloads
```
```
git clone https://gitbox.apache.org/repos/asf/ofbiz-framework.git ofbiz-framework
```
```
cd ofbiz-framework
```
```
git fetch --all --tags
```
```
git checkout release18.12.05
```

Then Inside Windows CMD type:
```
cd Downloads/ofbiz-framework
```
```
gradlew "ofbiz --load-data readers=seed,seed-initial" loadAdminUserLogin -PuserLoginId=admin
```

After finish building, type:

```
gradlew ofbiz 
```

To log into OFBiz, navigate with your browser to
https://localhost:8443/accounting
and login with username "admin" and password "ofbiz"

### Resources
https://ofbiz.apache.org/developers.html
