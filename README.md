# install JDK in Ubuntu
  + [oracle JDK](#oracle)
  + [open JDK](#open)
  + [Default JDK](#default)
  + [Select Alternative Version](#configure)
  + [Verify / Check](#verify)
***
## Oracle
- Oracle JDK
  + Download Letest JDK from [Oracle ⇩](https://www.oracle.com/java/technologies/javase-downloads.html) in TAR.GZ format
  + VERSION    : `8u301`  /  `11.0.12`  /  `16.0.2`
  + OS_VERSION : `aarch64`  /  `x64`
    - Step 1 : `mkdir`
      - Make Java Virtual Machine (JVM) Directory 
        ```bash
        sudo mkdir -p /usr/lib/jvm
        ```
    - Step 2 : `tar zxvf`
      - Extract Downloaded Tar.GZ file 
        ```bash
        sudo tar zxvf /Downloads/jdk-`VERSION`_linux-`OS_VERSION `_bin.tar.gz -C /usr/lib/jvm
        ```
    - Step 3 : Install
      - java
        ```bash
        sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-`VERSION`/bin/java 1
        ```
      - javac
        ```bash
        sudo update-alternatives --install /usr/bin/javac javac /usr/lib/jvm/jdk-`VERSION`/bin/javac 1
        ```
    - Step 4 : Set
      - java
        ```bash
        sudo update-alternatives --set java /usr/lib/jvm/jdk-`VERSION`/bin/java
        ```
      - javac
        ```bash
        sudo update-alternatives --set javac /usr/lib/jvm/jdk-`VERSION`/bin/javac
        ```
***
## Open
- Open JDK
  + VERSION : `8`  /  `11`  /  `13`  /  `14`  /  `16`
    ```bash
    sudo apt install openjdk-`VERSION`-jdk -y
    ```
***
## Default
- Defalut JDK
  ```bash
  sudo apt install default-jdk -y
  ```
***
## Configure
- Select Alternative Version
  + java
    ```bash
    sudo update-alternatives --config java
    ```
  + javac
    ```bash
    sudo update-alternatives --config javac
    ```
***
## verify
- Verify / Check Version 
  - java
    ```bash
    java --version
    ```
  - javac
    ```bash
    javac --version
    ```
***
