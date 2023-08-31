---
marp: true
theme: uncover
class: invert
---

# Global Protect and SSH

---

# About Me

---

# Global Protect

---

#### What is Global Protect Why do I need it?
* Global Protect is the Campus VPN
* Helps to secure our campus network, preventing outside parties from accessing internal assets

---

### How do I install it?
Go to vpn.csuchico.edu, log in, then choose the matching file for your OS, and install

--- 

### How do I install it on Linux?
Visit wiki.charon.click/vpn to view the community documentation for getting connected

---

# SSH

---

### What is SSH? Why do I need it?
* SSH is a secure way to connect to a remote server, using secure keys to verify the identity of the server and user
* SSH is the method used to connect to ECC-Linux

---

### Connecting to ECC-Linux

After connecting to Global Protect, you can enter this in your terminal to connect

```bash
$ ssh <username>@ecc-linux.csuchico.edu
```

---

# Additional SSH Tricks

---

### Log into ECC-Linux without a Password

```bash
$ ssh-keygen -t rsa -b 4096
$ ssh-copy-id <username>@ecc-linux.csuchico.edu
```

---

### SSH Tunneling 

```bash
ssh -ND 9999 <username>@ecc-linux.csuchico.edu
```

After running this, you will have a proxy that you can route your browser traffic through

---

# Help Session