![image of ssh key](./assets/SSH/SSHKey.png)

# How to add a new SSH key to your GitHub account using github.com 


<br />



## Table of Contents
|    |     |
|----------|:-------------:
| Task 1 |  Check for existing SSH keys
| Task 2 |    Generate a new SSH key and adding it to the ssh-agent
| Task 3 |  Adding a new SSH key to your GitHub Account

<br />



## Introduction

These instructions are on how to check for existing SSH keys, generate a new SSH key by adding it to the ssh-agent, and at last adding a new SSH key to your GitHub account. An SSH key is an alternate way to identify yourself when working with a GitHub repository that **_doesn't_** require you to enter your username and password every time.

<br />

## How an SSH Key Works

SSH keys come in pairs, a public key that gets shared with services like GitHub, and a private key that is stored on your local machine. If the keys match, you're granted access. The  cryptographic characteristic behind SSH keys ensures maximum security.  

<br />

## Prerequisites

<br />

### _To follow these instructions, you will need:_
- Mac Operating System
- GitHub Account
- Basic knowledge working with the terminal

<br />

### _Before adding a new SSH key to your GitHub account, you should have:_

<br >

- Checked for existing SSH keys
- Generated a new SSH key and added it to the ssh-agent

<br />
<br />

 <span style="font-family:papyrus; font-size:3em; color:green">
Task 1 - Check for existing SSH keys
 </span>

<br>
<br>
The first step to adding a new SSH key to your GitHub Account is checking to see if you have any existing SSH keys.

1. Open Terminal

2. Enter "ls -al ~/.ssh" to see if existing SSH keys are present (_This command lists the files in your .ssh directory, if they exist_)

    >$ ls -al ~/.ssh
 Lists the files in your .ssh directory, if they exist

3. Check the directory output to see if you already have a public SSH key. The filenames of the public keys are one of the following:

- id_rsa.pub (_most common_)
- id_ecdsa.pub
- id_ed25519.pub

If you don't see an existing public and private key pair, then you can generate a new SSH key.

---
**Tip:**

<mark>If you receive an error that ~/.ssh doesn't exist, don't worry! We'll create it when we generate a new SSH key.

---

<br>
<br>


 <span style="font-family:papyrus; font-size:3em; color:green">
Task 2 - Generate a new SSH key and adding it to the ssh-agent
 </span>

