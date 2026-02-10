# The UPMEM DPU SDK (v2023.1.0)

This repository contains **UPMEM-DPU SDK version 2023.1.0** (currently unavailable on the official UPMEM website).

---

## Notes before starting

This document expects the reader to already know the **DPU architecture**.

---

## Toolchain purpose

The **UPMEM DPU toolchain** is designed to meet the following requirements:

- Creating the programs embedded on **DPUs**
- Creating the **host application** that will drive the DPU programs
- Debugging both the **host application** and the **DPU programs**

To achieve this, the toolchain provides:

- A C compiler to build DPU programs: `dpu-upmem-dpurte-clang`
- A **Runtime Library** for DPU programs
- A **Host Library** to build DPU-enabled host applications
- A debugger for both host application and DPU programs: `dpu-lldb`

---

## Installing the UPMEM DPU toolchain

The UPMEM DPU toolchain has versions qualified on Linux for the following distributions:

- **Debian 10 (buster)** *(Recommended)*
- CentOS 7
- CentOS 8
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS

---

## Dependencies

### Python

The debugging tools use Python-based helpers and scripts. It is recommended to have **Python 3.x** installed.

Example install (Ubuntu):

```bash
apt install python3

git clone https://github.com/CMU-SAFARI/UPMEM

source "$HOME/upmem-sdk/upmem_env.sh"
