# Hadoop and Hive Setup on Windows 🖥️

This repository documents the step-by-step process of setting up Hadoop and Hive on a Windows system. It includes all the configurations, commands, and troubleshooting tips.

## 🌟 Key Highlights
- **Hadoop Setup:** Configuring HDFS and running distributed computations.
- **Hive Setup:** Installing Hive and integrating it with Hadoop.
- **Troubleshooting:** Solutions to common issues faced during the setup.

---

## 🛠️ Prerequisites
- **Software Requirements:**
  - [Java JDK 8](https://www.oracle.com/in/java/technologies/javase/javase8-archive-downloads.html)
  - [Hadoop 3.2.4](https://hadoop.apache.org/release/3.2.4.html)
  - [Apache Hive 3.1.2](https://archive.apache.org/dist/hive/hive-3.1.2/)

---

## 📜 Steps
1. [Java Installation](#java-installation)
2. [Hadoop Installation](#hadoop-installation)
3. [Hive Installation](#hive-installation)
4. [Testing Your Setup](#testing-your-setup)
5. [Troubleshooting](#troubleshooting)

---

## 📁 Directory Structure
- `README.md`: Main documentation.
- `config-files/`: Configuration files like `core-site.xml` and `hive-site.xml`.

---

## 🚀 Getting Started
Follow the detailed steps in this README to complete your setup successfully.

---
## ☕ Java Installation

### **Step 1: Download Java JDK**
1. Visit the [Java JDK 8+ Download Page](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html).
2. Select the appropriate version for your Windows system:
   - **x64 Installer** for 64-bit Windows.
   - **x86 Installer** for 32-bit Windows.
3. Download the `.exe` file and run the installer.

### **Step 2: Install Java**
1. Follow the installer prompts:
   - **Choose Installation Directory**: Instead of the default directory, create a new folder in the `C:` drive named `Java` (e.g., `C:\Java`).
   - Avoid installing in `Program Files` to prevent issues caused by spaces in the path.
   - Complete the installation process.
2. After installation, note the installation path (e.g., `C:\Java\jdk-<version>`).

### **Step 3: Set Environment Variables**
1. Open **Control Panel** → **System** → **Advanced System Settings** → **Environment Variables**.
2. Under **System Variables**, click **New**:
   - **Variable Name**: `JAVA_HOME`
   - **Variable Value**: Path to your JDK folder (e.g., `C:\Java\jdk-<version>`).
3. Edit the `Path` variable:
   - Add `%JAVA_HOME%\bin` to the list.

### **Step 4: Verify Installation**
1. Open a Command Prompt (`Win + R`, then type `cmd`).
2. Run the command:
   ```bash
   java -version
   javac -version
   ```
### Expected Outputs

#### **Command:** `java -version`
```plaintext
java version "1.8.0_431"
Java(TM) SE Runtime Environment (build 1.8.0_431-b10)
Java HotSpot(TM) 64-Bit Server VM (build 25.431-b10, mixed mode)
```

#### **Command:** `java -version`
```plaintext
javac 1.8.0_431
```
   
### **🛠️ Troubleshooting**
If java -version does not work:
  - Ensure the JAVA_HOME path is correct.
  - Ensure %JAVA_HOME%\bin is added to the Path variable.

---
Happy Coding 🪄
