# Pwn (二进制漏洞利用)

**方向解释：**
Pwn 是 CTF 中难度较高的方向，主要针对二进制程序中的内存破坏漏洞（如缓冲区溢出、格式化字符串漏洞、堆溢出等），编写利用脚本（Exploit）劫持程序控制流，最终获取远程服务器的 Shell 或读取 Flag。

**需要的学习内容：**
*   **基础知识**：深入理解内存管理（栈、堆）、函数调用约定、ELF/PE 文件格式。
*   **漏洞类型**：
    *   栈溢出 (Stack Overflow)。
    *   格式化字符串漏洞 (Format String)。
    *   堆溢出 (Heap Overflow) 及堆管理机制 (glibc heap)。
    *   整数溢出。
*   **保护机制与绕过**：NX/DEP, ASLR, PIE, Canary, RELRO。
*   **Shellcode 编写**。
*   **工具**：pwntools (Python 库，必备), GDB + pwndbg/peda/gef, ROPgadget, one_gadget。
