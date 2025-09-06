
# Install Java JDK 25 on macOS (directly from this link)

Download from: [OpenJDK 25 Early Access](https://jdk.java.net/25/)

---

## Available Builds

- **macOS AArch64 (M1/M2/M3 chips):**  
  File: `openjdk-25_macos-aarch64_bin.tar.gz`  
  Size: `215390344`  

- **macOS x64 (Intel):**  
  File: `openjdk-25_macos-x64_bin.tar.gz`  
  Size: `217677049`  

---

## Installation Steps (for both AArch64 and x64) (dowload by terminal)

1. **Download the correct file for your architecture**  
   Example (for Apple Silicon):
   ```bash
   curl -O https://download.java.net/java/early_access/jdk25/36/GPL/openjdk-25_macos-aarch64_bin.tar.gz
   ```

   Example (for Intel):
   ```bash
   curl -O https://download.java.net/java/early_access/jdk25/36/GPL/openjdk-25_macos-x64_bin.tar.gz
   ```

2. **Extract the downloaded file**
   ```bash
   tar -xzf openjdk-25_macos-*_bin.tar.gz
   ```

3. **Move it to the Java Virtual Machines directory**
   ```bash
   sudo mv jdk-25.jdk /Library/Java/JavaVirtualMachines/
   ```

4. **Configure environment variables**  
   Open your `~/.zshrc` (or `~/.bashrc` if using bash) and add:
   ```bash
   export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-25.jdk/Contents/Home
   export PATH=$JAVA_HOME/bin:$PATH
   ```

5. **Reload shell configuration**
   ```bash
   source ~/.zshrc
   ```

6. **Verify installation**
   ```bash
   java --version
   ```

   **Expected output:**
   ```
   openjdk 25 2025-09-16
   OpenJDK Runtime Environment (build 25+36-3489)
   OpenJDK 64-Bit Server VM (build 25+36-3489, mixed mode, sharing)
   ```
````
