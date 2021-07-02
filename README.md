# Nand2Tetris

The following are my install notes from the nand2tetris project. The project website is [here](https://www.nand2tetris.org/) this the definitive source for notes and project resources _(outside of the book Elements of Computing Systems)_.

## Install

https://www.nand2tetris.org/software

Download and install the zip package, installed under this parent directory into

```
├── README.md
└── nand2tetris
    ├── projects
    └── tools
```

## Execute the built in tools

First we ensure we have java installed by running

```sh
java -version
# OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.7+10)
# OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.7+10, mixed mode)
```

To make executing these files easy, lets put the source directory for tools on PATH.

```sh
echo "export PATH=\$PATH:$PWD/nand2tetris/tools" >> ~/.zshrc ; source ~/.zshrc
```

We also need to set the proper permissions for the nand2tetris tools

```sh
chmod 744 nand2tetris/tools/*.sh
```

## Tools

nand2tetris includes the following programs:

- Assembler.sh
- CPUEmulator.sh
- HardwareSimulator.sh
- JackCompiler.sh
- TextComparer.sh
- VMEmulator.sh
