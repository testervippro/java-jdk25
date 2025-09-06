
# Install Java JDK 25 on macOS (using SDKMAN!)

SDKMAN! makes it easy to install and switch between multiple JDK versions on macOS.

---

## Installation Steps

1. **Install SDKMAN!** (if not already installed)

   ```bash
   curl -s "https://get.sdkman.io" | bash
   source "$HOME/.sdkman/bin/sdkman-init.sh"
   sdk version
   ```

2. **List available JDKs**

   ```bash
   sdk list java
   ```

   You will see something like:

   ```
   ...
   |     | 25.ea.36     | open    |            | 25.ea.36-open
   ...
   ```

3. **Install JDK 25 (Early Access build)**

   ```bash
   sdk install java 25.ea.36-open
   ```


4. **Verify installation**

   ```bash
   java --version
   ```

   **Expected output:**

   ```
   openjdk 25 2025-09-16
   OpenJDK Runtime Environment (build 25-ea+36-...)
   OpenJDK 64-Bit Server VM (build 25-ea+36-..., mixed mode, sharing)
   ```


