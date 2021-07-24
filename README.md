# install JDK in Ubuntu
  # [oracle](#oracle jdk & jre)
  # [open](#open jdk)
## Oracle JDK & JRE
Download Letest JDK [⇩](https://www.oracle.com/java/technologies/javase-downloads.html) in Tar.GZ format
+ Step 1 :
  - Make Java Virtual Machine (JVM) Directory 
  ```bash
  sudo mkdir -p /usr/lib/jvm
  ```
+ Step 2 :
  - Extract Downloaded Tar.GZ file 
  ```bash
  sudo tar zxvf /Downloads/jdk-`VERSION`_`OS_VERSION `_bin.tar.gz -C /usr/lib/jvm
  ```
+ Step 3 : Install JDK 
  - java
  ```bash
  sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk-`VERSION`/bin/java" 1
  ```
  - javac
  ```bash
  sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk-`VERSION`/bin/javac" 1
  ```
+ Step 4 : Set JDK
  - java
  ```bash
  sudo update-alternatives --set java /usr/lib/jvm/jdk-`VERSION`/bin/java
  ```
  - javac
  ```bash
  sudo update-alternatives --set javac /usr/lib/jvm/jdk-`VERSION`/bin/javac
  ```
+ Step 5 : Verify / Check Version 
    - java
    ```bash
    java --version
    ```
    - javac
    ```bash
    javac --version
    ```
## Open JDK
+ Step 1 :
  - JDK
  ```bash
  sudo apt install openjdk-`VERSION`-jdk -y
  ```
  - JRE
  ```bash
  sudo apt install openjdk-`VERSION`-jre -y
  ```
    
    
    
