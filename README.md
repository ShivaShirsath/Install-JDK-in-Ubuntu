# install JDK in Ubuntu
## Oracle JDK & JRE
Download Letest JDK [⇩](https://www.oracle.com/java/technologies/javase-downloads.html) in Tar.GZ format
- Step 1 :
  > Make Java Virtual Machine (JVM) Directory 
  ```bash
  sudo mkdir -p /usr/lib/jvm
  ```
- Step 2 :
  > Extract Downloaded Tar.GZ file 
  ```bash
  sudo tar zxvf /Downloads/jdk-'VERSION'-linux-x64.tar.gz -C /usr/lib/jvm
  ```
