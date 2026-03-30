# Hydra Brute Force Lab Report

A simple cybersecurity lab report demonstrating password guessing attempts with Hydra in a controlled local environment for educational purposes.

## Author
**Name:** Muhammad Tukur Muhammad

## Project Title
**What is a Brute Force Attack? How Can You Prevent It?**

## Objective
The purpose of this lab is to demonstrate how a brute force attack works in a controlled environment and to explain why strong passwords and proper authentication controls are important.

## Tool Used
- Kali Linux
- Hydra
- Nano Text Editor
- OpenSSH Server

## Lab Environment
This demonstration was carried out in a local lab environment on Kali Linux.  
The target used was a local SSH service running on the same machine.  
No external system or third-party network was involved.

## Steps Performed

### 1. Created a Password Wordlist
A password list was created using Nano and saved as `passwords.txt`.

Example passwords used:
- 123456
- password
- admin
- admin123
- letmein
- secure2026

![Wordlist Creation](screenshots/01-wordlist-created.png)

### 2. Verified the SSH Service
The SSH service status was checked to confirm the service was available locally.

![SSH Status](screenshots/02-ssh-status.png)

### 3. Ran Hydra Against the Local Test Service
Hydra was executed against the local SSH service using the prepared password list.

![Hydra Run](screenshots/03-hydra-run.png)

### 4. Observed the Result
Hydra completed the password attempts and returned the result.

![Hydra Result](screenshots/04-result.png)

## Observation
The result showed that the passwords in the wordlist did not match the actual account password.  
This demonstrates that when a strong or unknown password is not present in a wordlist, brute force attempts may fail.

## Key Lesson
This lab shows that weak passwords are easier to guess, while stronger passwords reduce the success of brute force attacks.

## Prevention Methods
- Use strong and unique passwords
- Enable multi-factor authentication
- Limit repeated login attempts
- Use CAPTCHA where applicable
- Monitor authentication logs
- Disable unnecessary remote services

## Conclusion
This lab successfully demonstrated the concept of a brute force attack in a safe local environment.  
It also showed the importance of password strength and other security controls in defending systems against automated password guessing.

## Educational Use Notice
This repository is intended strictly for educational documentation of authorized local lab testing.
