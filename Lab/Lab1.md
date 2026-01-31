# Experiment 1: Compare Virtual Machines with Containers

**Name:** [Raghav Sharma]  
**Roll No:** [R2142230283]  
**Course:** Containerization and DevOps  
**Date:** [31/1/2026]

---

## 1. Objective
To study and compare the architectural and functional differences between Virtual Machines (VMs) and Containers (e.g., Docker).

## 2. Theory

### Virtual Machines (VM)
A Virtual Machine is a digital version of a physical computer. It runs on a software called a **Hypervisor** (Type 1 or Type 2).
- **Key Characteristic:** Every VM includes a full "Guest Operating System," its own binaries, and libraries. This makes them heavy but fully isolated.

### Containers
Containers are lightweight packages of application code together with dependencies (libraries, frameworks). They do not bundle a full OS; instead, they share the **Host OS Kernel**.
- **Key Characteristic:** Containers are process-level isolations. They start instantly and use a fraction of the memory a VM would use.

## 3. Comparison

| Feature | Virtual Machines (VM) | Containers |
| :--- | :--- | :--- |
| **Architecture** | Hypervisor-based; each VM has a full Guest OS. | Daemon-based; shares the Host OS kernel. |
| **Size** | Heavyweight (Gigabytes). | Lightweight (Megabytes). |
| **Boot Speed** | Slow (Minutes) - Requires OS boot. | Fast (Seconds) - Starts as a process. |
| **Isolation** | Strong (Hardware-level isolation). | Moderate (Process-level isolation). |
| **Portability** | Harder to migrate (large snapshots). | Highly portable (run anywhere Docker runs). |
| **Resource Usage** | High dedicated resources (RAM/CPU). | Efficient; resources are released when not in use. |

## 4. Diagrammatic Representation (Optional)
*(You can describe the architecture here or insert an image link if you have one)*

- **VM:** Hardware -> Hypervisor -> Guest OS -> App
- **Container:** Hardware -> Host OS -> Container Engine -> App

## 5. Conclusion
In this experiment, we analyzed the differences between virtualization and containerization.
- **VMs** are best suited for running multiple different OSs (e.g., Linux on Windows) and apps requiring total isolation.
- **Containers** are superior for microservices, DevOps workflows, and scenarios requiring fast deployment and scalability.

---