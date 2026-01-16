# File-Integrity-Checker-
The File Integrity Checker calculates SHA-256 hashes for every file in a chosen folder to detect changes. It uses Python’s os module to list files and hashlib to generate secure hashes. By comparing hashes from different runs, users can spot modified, added, or deleted files, making it a simple integrity-monitoring tool.
COMPANY: CODTECH IT SOLUTIONS
NAME: KAUSHAL M LEMBHE
INTERN ID: CTIS1154
DOMAIN: CYBER SECURITY AND ETHICAL HACKING 
DURATION: 4 WEEKS 
MENTOR: NEELA SANTOSH 

DESCRIPTION OF THE TASK:
File Integrity Checker – Full Task Description (Under 350 Words)

The objective of this task is to understand file integrity verification using SHA-256 hashing. File integrity checking is an important cybersecurity concept used to confirm that a file has not been modified, corrupted, or tampered with. In this task, we create a Python program that calculates the SHA-256 hash value of every file in a selected directory. This hash can later be compared with the original hash to ensure that the file is authentic and unchanged.

We first obtained an example hash value from the official Kali Linux website. While downloading Kali Linux ISO images, the website displays the SHA-256 checksum so that users can verify whether their downloaded file is genuine. This ensures that the file has not been altered or infected during download. In the screenshot, the Kali website shows SHA-256 values like:

3b4a3a9f5fb6532635800d3eda94414fb69a44165af6db6fa39c0bdae750c266

This demonstrates how real-world platforms use hashing for integrity verification.

To replicate this concept, we created a Python program. The program uses two built-in modules: os, to navigate through directories and list files, and hashlib, to generate SHA-256 cryptographic hashes. SHA-256 is a strong algorithm that produces a unique 64-character hash for any file. Even a one-byte change in the file generates a totally different hash, making it effective for detecting tampering.

The program has two main functions. The calculate_sha256() function opens each file in binary mode and reads it in 65,536-byte chunks. This prevents memory overload and ensures large files can be hashed efficiently. The check_integrity() function validates the directory path and uses os.walk() to visit every file in the directory. For each file, it calculates the SHA-256 hash and prints the result.

By comparing the generated hash values with the original ones—just like checking the Kali Linux ISO hash—users can confirm whether files are safe and unchanged. This task gives practical experience in implementing and understanding file integrity verification using hashing.
