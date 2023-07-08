# Morphgen

## RISC-V

Implementing a Processor using the [RISC-V](https://riscv.org/wp-content/uploads/2017/05/riscv-spec-v2.2.pdf) instruction set. 

### CPU

For testing the **cpu**, clone and build the `riscv-tests`. The tests can be found in the modules/ folder. 
Please follow along the installation [guide](modules/README.md).

Run the tests via:
```bash
python riscv_cpu.py
```

### Assembler 

Run the Assembler via:
```bash 
python riscv_asm.py testfs/riscv_minimal.s
``` 

## ARM

**Prequisits**: Cross-Compiler (if you are not on a ARM architecture anyway)
```bash
sudo apt install gcc gcc-arm-linux-gnueabi binutils-arm-linux-gnueabi gcc-aarch64-linux-gnu binutils-aarch64-linux-gnu make
```

### ARM Assembler
```bash
python arm_asm.py testfs/subtract.s
```

Run the bash script to investigate the desired out of the assembler.
```bash
./run_arm32_tests.sh
```

### Additional Material

Source -> Preprocessor -> Compiler -> assembly (.asm) -> Assembler -> object (.o) -> (+ Libraries) Linker -> Executable

#### ARMv

#### RISC-V

- Course: [Computer Systems Organization](https://nyu-cso.github.io/index.html)
- [Unofficial RISC-V Manual](https://jemu.oscc.cc/): Additional manuscript about RISC-V along the official RISC-V Manual.
- [riscv-isadoc](https://msyksphinz-self.github.io/riscv-isadoc/html/index.html): Instruction Set docs on Github.
