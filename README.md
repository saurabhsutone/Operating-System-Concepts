# Operating System Concepts

## Introduction
This repository provides a comprehensive explanation of operating system (OS) concepts with examples covering **Windows, Linux, and macOS**. It includes detailed discussions on **kernels, process management, memory management, file systems, I/O systems, virtualization, and security**.

---

## 1. What is an Operating System?
An operating system (OS) is system software that manages computer hardware and software resources, providing services for computer programs.

### Key Functions:
- Process Management
- Memory Management
- File System Management
- Device Management
- User Interface (CLI/GUI)

---

## 2. Kernel
The **kernel** is the core part of an OS, responsible for managing system resources and communication between hardware and software.

### Types of Kernels:
1. **Monolithic Kernel** (e.g., Linux) - All OS services run in kernel mode.
2. **Microkernel** (e.g., macOS, Windows NT) - Only essential services run in kernel mode, improving stability.
3. **Hybrid Kernel** (e.g., Windows) - A mix of monolithic and microkernel architectures.

### Kernel Comparison:
| Feature         | Windows (Hybrid) | Linux (Monolithic) | macOS (Microkernel + Monolithic) |
|---------------|----------------|------------------|--------------------------|
| Performance   | Moderate       | High             | Moderate                 |
| Stability     | Good           | Very Good        | Excellent                 |
| Security      | High           | High             | High                      |

---

## 3. Process Management
Processes are instances of executing programs.

### Example:
**Linux:** Check running processes
```bash
ps aux | grep process_name
```
**Windows:** Check running processes
```powershell
tasklist | findstr process_name
```

---

## 4. Memory Management
Memory management involves allocating and deallocating RAM for processes.

### Example:
**Linux:** Check memory usage
```bash
free -h
```
**Windows:** Check memory usage
```powershell
typeperf "\Memory\Available MBytes"
```

---

## 5. File System
Each OS has its own file system structure.

| OS       | File System   |
|----------|--------------|
| Windows  | NTFS, FAT32  |
| Linux    | EXT4, XFS    |
| macOS    | APFS, HFS+   |

### Example:
**Linux:** List files in a directory
```bash
ls -l
```
**Windows:** List files in a directory
```powershell
dir
```

---

## 6. Input/Output System
Handles communication between applications and hardware devices.

### Example:
**Linux:** Check connected devices
```bash
lsblk
```
**Windows:** Check connected devices
```powershell
Get-PnpDevice
```

---

## 7. Virtualization
Virtualization allows running multiple OS instances on a single machine.

### Example:
**Linux:** Create a virtual machine using KVM
```bash
virt-install --name myvm --memory 2048 --vcpus 2 --disk size=20G
```
**Windows:** Enable Hyper-V
```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V-All
```

---

## 8. Security in OS
Security features prevent unauthorized access and system threats.

### Example:
**Linux:** Check open ports
```bash
netstat -tulnp
```
**Windows:** Check open ports
```powershell
netstat -ano
```

---

## Conclusion
This repository serves as a guide to OS concepts, providing practical examples for Windows, Linux, and macOS. Contributions and improvements are welcome!

## License
[MIT License](LICENSE)

