# install JDK in Ubuntu
  + [oracle JDK](#oracle)
  + [open JDK](#open)
  + [Select Alternative Version](#configure)
  + [Verify / Check](#verify)
***
## Oracle
+ Download Letest JDK from [Oracle ⇩](https://www.oracle.com/java/technologies/javase-downloads.html) in TAR.GZ format
  - VERSION    : `8u301`  /  `11.0.12`  /  `16.0.2`
  - OS_VERSION : `aarch64`  /  `x64`
    + Step 1 : `mkdir`
      - Make Java Virtual Machine (JVM) Directory 
        ```bash
        sudo mkdir -p /usr/lib/jvm
        ```
    + Step 2 : `sudo tar zxvf`
      - Extract Downloaded TAR.GZ file 
        ```bash
        sudo tar zxvf /Downloads/jdk-`VERSION`_linux-`OS_VERSION `_bin.tar.gz -C /usr/lib/jvm
        ```
    + Step 3 : Install
      - java
        ```bash
        sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-`VERSION`/bin/java 1
        ```
      - javac
        ```bash
        sudo update-alternatives --install /usr/bin/javac javac /usr/lib/jvm/jdk-`VERSION`/bin/javac 1
        ```
    + Step 4 : Set
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
+ VERSION
  - `default-jdk`
  -  `openjdk-8-jdk`
  -  `openjdk-11-jdk`
  -  `openjdk-12-jdk`
  -  `openjdk-13-jdk`
  -  `openjdk-14-jdk`
  -  `openjdk-15-jdk`
  -  `openjdk-16-jdk` 
  -  `openjdk-17-jdk`  
  ‎
  ```bash
  sudo apt install `VERSION`
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
## Verify
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
