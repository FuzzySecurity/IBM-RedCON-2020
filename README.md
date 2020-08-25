# IBM RedCON 2020: Throwing an AquaWrench into the Kernel :zap::skull:

### What is AquaWrench?

AquaWrench bridges the gap between Administrator and Kernel access. It is a modular plug-and-play framework built around vulnerable signed drivers that allow the user to map and unmap physical memory. Through this exploitation primitive AquaWrench has the ability to perform arbitrary Kernel reads and writes.

### What can AquaWrench do?

AquaWrench is still in development as such it is not feature-complete. Some of the capabilities currently in AquaWrench are:

  - Manipulate the PS_PROTECTION status of any PID.
  - Duplicate handles from any source process to any target process.
  - Dynamically disable driver signing requirements in-memory.
  - Load unsigned Kernel drivers into memory.
  - Reflective driver loading (work-in-progress).
  - List/manipulate Kernel notification routines.
  - Give the user the ability to perform arbitrary Kernel DWORD/QWORD read and write.
  - Sinkhole ETW trace data from the Kernel.

### What OS'es does AquaWrench support?

As with any Kernel based tradecraft, compatibility and stability are of primary concern. All functionality in AquaWrench has been gated behind **ntdll!RtlGetVersion** checks. Currently, all functionality in AquaWrench has been certified to work on the following OS'es (where applicable):

  - Win7, Win8, Win8.1, Win10 (1507, 1511, 1607, 1703, 1709, 1803, 1809, 1903)
  - 2k8R2, 2k12, 2k12R2, 2k16, 2k19

### Demos

  * IBM RedCON 2020: AquaWrench Demo 1 (Protected Processes) - https://www.youtube.com/watch?v=zoFRBJp5b94
  * IBM RedCON 2020: AquaWrench Demo 2 (Driver Signing Bypass) - https://www.youtube.com/watch?v=Hv3XM_eGcCU
  * IBM RedCON 2020: AquaWrench Demo 3 (Blinding Telemetry) - https://www.youtube.com/watch?v=KjPCXWFsECE
  
### Recording

A full recording of the presentation is also available at the following URL:
https://gateway.on24.com/wcc/eh/2170362/category/36001/red-con-2020
