# Apache Nifi Learnings

## Requirements:
### 1. Download and Install Apache NiFi:
Download the NiFi binary from here based on your requirements.
### 2. Install NiFi on macOS:
#### 2.1 Download and Install Java (macOS):
Download Java SDK based on your system requirements and install it. You can choose to download it from Oracle or use Homebrew.
Example using Homebrew:
```
brew install openjdk
```
```
brew install openjdk@11 ## for a specific version
```
#### 2.2 Set up JAVA_HOME:
Check if Java is already installed:
```
java -version
```
Create the zshenv file:
```
touch ~/.zshenv
```
Find the installation path of your Java SDK:
```
/usr/libexec/java_home ## /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home
```
Set JAVA_HOME:
```
open ~/.zshenv
## Write and save
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home
source ~/.zshenv
```
Verify if JAVA_HOME is set up correctly:
```
echo $JAVA_HOME 
# This should give the result - 
/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home
```
### 3. Start Apache NiFi:
Move to the folder where NiFi is installed:
```
cd <your_path>/nifi-1.23.2
bin/nifi.sh start
```





