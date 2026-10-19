
# flistgen

A lightweight, standalone GUI utility that automatically parses, sorts, and separates Verilog and SystemVerilog files into perfectly ordered compilation filelists (`rtl_filelist.f` and `tb_filelist.f`).

## Why?

Because life is too short to manually track module dependencies and maintain filelists for an Euclide-based project flow. `flistgen` automates the grunt work of compilation ordering so you can focus on actual RTL development and verification. 

## Features

* **Zero Dependencies:** Distributed as a standalone Linux executable. No Python, Tkinter, or external packages required on the host machine.
* **Automatic Dependency Resolution:** Parses code for `module`, `class`, `package`, and `interface` definitions to build a dependency graph and topologically sort files bottom-up.
* **Smart TB/RTL Separation:** Automatically identifies testbench files and routes them to `tb_filelist.f` based on directory paths (`/tb/`, `/uvm/`), filenames, and UVM/SV syntax heuristics. 
* **GUI-Driven:** Select all your source files at once through a clean, intuitive interface.

## Usage

1. **Download** the `flistgen` executable.
2. **Make it executable** via your terminal:
   ```bash
   chmod +x ./flistgen
   ```
#### Note: Used AI to Create this README :) cause don't wanna blabber
