# PassROOT: Root Password Changer

## Overview

A simple tool designed to change the password for the root user on Unix-based systems. It demonstrates a potential security vulnerability by exploiting unauthorized write access to the `/etc/passwd` file.

## Usage

1. **Write Access Check:**
   - The script checks if it has write access to the `/etc/passwd` file.

2. **Password Change:**
   - If write access is granted, the user is prompted to enter a new password for the root user.

3. **Encryption:**
   - The new password is encrypted using the `crypt` module.

4. **Update `/etc/passwd`:**
   - The script updates the `/etc/passwd` file with the new encrypted password for the root user.

5. **Launch New Shell:**
   - The script attempts to launch a new shell as ROOT.

## How to Run

```bash
python passROOT.py
