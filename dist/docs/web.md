# Web (Web 安全)

**方向解释：**
Web 安全是 CTF 中最常见的方向，主要通过浏览器或脚本与 Web 服务器进行交互，寻找 Web 应用程序中的漏洞（如 SQL 注入、XSS、文件包含、命令执行等）来获取 Flag。

**需要的学习内容：**
*   **基础知识**：HTTP/HTTPS 协议、HTML/CSS/JavaScript、浏览器开发者工具。
*   **编程语言**：PHP（最常见）、Python、Go、Java、SQL。
*   **常见漏洞**：
    *   OWASP Top 10（SQL注入、XSS、CSRF、XXE、SSRF 等）。
    *   文件上传/包含漏洞。
    *   反序列化漏洞（PHP, Java, Python）。
    *   模板注入 (SSTI)。
*   **工具**：Burp Suite、Postman、sqlmap、dirsearch。
*   **框架**：了解常见 CMS (WordPress, Discuz) 和框架 (Flask, Django, Spring Boot, ThinkPHP) 的特性及历史漏洞。
