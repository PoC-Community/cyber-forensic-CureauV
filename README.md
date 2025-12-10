# **Workshop PoC : Forensic**

## 🔍 **Introduction**

In this workshop, you’ll step into the **role of a forensic analyst** tasked with examining a vmss.core file captured from a suspicious Windows virtual machine.

**Your mission is to explore this snapshot, reconstruct user activity, identify malicious behavior, and extract hidden information.**

Snapshot link : 
- <https://epitechfr-my.sharepoint.com/:u:/g/personal/yoel_edery_epitech_eu/EXolIqXtDU5Ds9N9kxSCY_IB0L7uGkme9BeBOkWstrkIpg?e=L6S7Z9> 
- <https://t.ly/5mU0>

Password : PoC_Workshop_Secu_Forensic_2021

## 🤓 **What You Will Learn**

* How to analyze a VMware memory snapshot (`vmss.core`).

* How to use **Volatility 3** to inspect system memory.

* How to identify users, processes, and network activity.

* How to extract and examine process memory dumps.

* How to recover hidden or malicious content from RAM.

* How to locate specific data inside a process (e.g., Python version).

## 🚚 **Delivery format**

As usual, the output format will be a **text file** containing the flags and the **reasoning** behind your solution.    


## 🎯 **Challenges**

### **🔹 Challenge 1 — Who uses this machine ?**

You’ve just recovered a computer and need to identify the active users.

**Expected flag :** `PoC{USERNAME1,USERNAME2}`

---

### **🔹 Challenge 2 — Suspicious connection**

Connections to `https://www.poc-innovation.fr/` were intercepted.  
Which process is responsible?

**Expected flag :** `PoC{PID + Owner}`

💡 : _The site has been requested several times._

---

### **🔹 Challenge 3 — Command line analysis**

Using the PID found earlier, extract the **full command line**, then compute its **SHA1 hash**.

**Expected flag :** `PoC{HASH(SHA1)}`

---

### **🔹 Challenge 4 — Process memory dump**

You spotted a malicious program. Create a **binary memory dump** of this process and compute its SHA512 hash.

**Expected flag :** `PoC{HASH(SHA512)}`

---

### **🔹 Challenge 5 — Memory address hunting**

I would like to find the **memory address** of the process that shows us the Python version.

A SHA384 hash of the decompressed dump is provided for verification:

```
eaf86b887f64c5db77d878645d78da544b52c00f76b3967a8128546a3740ad443994d08166e6b5b071def6a63d776d45
```

**Expected flag :** `PoC{MemoryAddress}`

<h2 align=center>
Organization
</h2>
<br/>
<p align='center'>
    <a href="https://www.linkedin.com/company/pocinnovation/mycompany/">
        <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn logo">
    </a>
    <a href="https://www.instagram.com/pocinnovation/">
        <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram logo"
>
    </a>
    <a href="https://twitter.com/PoCInnovation">
        <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter logo">
    </a>
    <a href="https://discord.com/invite/Yqq2ADGDS7">
        <img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Discord logo">
    </a>
</p>
<p align=center>
    <a href="https://www.poc-innovation.fr/">
        <img src="https://img.shields.io/badge/WebSite-1a2b6d?style=for-the-badge&logo=GitHub Sponsors&logoColor=white" alt="Website logo">
    </a>
</p>

> 🚀 Don't hesitate to follow us on our different networks, and put a star 🌟 on `PoC's` repositories.
