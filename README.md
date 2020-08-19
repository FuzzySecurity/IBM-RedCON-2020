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

The presentation has three demos, I will add the recordings for those next week.
