# RISC-V 32-bit Toolchain

This repository provides prebuilt RISC-V GCC toolchains for `riscv32-unknown-elf` with support for multiple GCC versions.

## Source  
This prebuilt toolchain is built from the **official RISC-V GNU Toolchain** without any modifications. It is provided solely for convenience.  

- **Upstream Repository:** [RISC-V GNU Toolchain](https://github.com/riscv-collab/riscv-gnu-toolchain)  
- **Upstream License:** [GNU General Public License (GPL v3)](https://www.gnu.org/licenses/gpl-3.0.html)  

This repository **only provides prebuilt binaries** and does not introduce any additional modifications or licensing terms beyond those of the upstream project.

## Toolchain Details
- **Target:** riscv32-unknown-elf
- **Architecture:** RV32IMZicsr

## Available Versions
This repository supports multiple versions of GCC. Replace `{VERSION}` with the desired version number when downloading the toolchain.

- Available versions:
  - 14.2.0
  - 13.2.0

## Download and Installation

1. Set the desired version
   ```
   VERSION={VERSION}
   ```

2. Download the prebuilt toolchain
    - **Linux**
    ```
    wget https://github.com/your-username/riscv32-toolchain/releases/download/v$VERSION/riscv32-toolchain-linux.tar.gz
    tar -xzvf riscv32-toolchain-linux.tar.gz -C /opt
    ```
    - **macOS**
    ```
    wget https://github.com/your-username/riscv32-toolchain/releases/download/v$VERSION/riscv32-toolchain-macos.tar.gz
    tar -xzvf riscv32-toolchain-macos.tar.gz -C /opt
    ```  
3. Add the toolchain to your `PATH`
   ```
   export PATH=/opt/riscv/bin:$PATH
   ```
4. Verify installation
   ```
   riscv32-unknown-elf-gcc --version
   ```

You can replace `{VERSION}` with the desired GCC version to install the corresponding toolchain.