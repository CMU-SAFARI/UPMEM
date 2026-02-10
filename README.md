**The UPMEM DPU SDK**

This repositry contains UPMEM-DPU SDK version 2023.1.2

Notes before starting

This document expects the reader to know the DPU architecture.

The toolchain purpose

The UPMEM DPU toolchain is designed to answer the following requirements:
Creating the programs embedded on DPUs
Creating the host application that will drive the DPU programs
Debugging both the host application and the DPU programs
To this intent, it provides the following tools:
A C compiler to build DPU programs: dpu-upmem-dpurte-clang
A Runtime Library for the DPU programs
A Host Library to create DPU-enabled host applications
A debugger for both host application & DPU programs: dpu-lldb
