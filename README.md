### 🛡️ Public Key Cryptography Basics

**Room:** [🛡️ Public Key Cryptography Basics — TryHackMe](https://tryhackme.com/room/publickeycrypto)  
**Status:** ✅ Completed  
**Date:** *28 May 2025*

---

### 🎯 Objective  
To understand how public key cryptography works and explore tools like RSA, Diffie-Hellman, digital signatures, and certificates — plus how these methods are used in protocols like SSH and TLS.

---

### 🗝️ Key Concepts  
- **Public Key Cryptography (Asymmetric)** – Uses a public/private key pair to encrypt and decrypt.
- **RSA** – Relies on the difficulty of factoring large prime numbers.
- **Diffie-Hellman** – Key exchange method allowing two parties to create a shared secret over an insecure channel.
- **Digital Signatures** – Use a private key to sign data and a public key to verify it.
- **Certificates** – Prove identity using trusted Certificate Authorities (CAs).
- **SSH** – Uses public key authentication for secure access to remote systems.
- **PGP/GPG** – Software for encrypting, signing, and securing files and emails using OpenPGP standard.

---

### 🛠️ Tools/Concepts Practised  
- **RSA Key Components:** p, q, n, e, d, m (message), c (ciphertext)
- **Diffie-Hellman Parameters:** g, p, A, B
- **ssh-keygen** – Key pair generation
- **GPG Commands:** `gpg --full-gen-key`, `gpg --import`, `gpg --decrypt`
- **SSH Configurations:** `authorized_keys`, `~/.ssh`, `ssh -i key user@host`

---

### ⚠️ Challenges Faced  
- Grasping the actual math behind RSA (especially modulo operations).
- Visualising how key exchange happens without ever sending the secret key.
- Understanding real-world uses of digital certificates and their trust chains.

---

### 🧠 What I Learned  
- RSA depends on the fact that multiplying primes is easy, but factoring is hard.
- Diffie-Hellman lets two parties create the same key without ever sharing it.
- SSH uses asymmetric encryption to identify servers and users without passwords.
- Digital signatures offer non-repudiation and integrity checks.
- TLS certificates are signed by trusted root CAs and form trust chains in browsers.

---

### 🌐 Real-World Application  
> Every HTTPS site uses TLS certificates, which rely on public key cryptography. SSH is used daily by sysadmins to securely manage remote machines. Digital signatures are vital in software updates, documents, and email verification.

---

### 💭 Reflections  
- It was helpful to walk through simplified maths behind RSA and DH to reinforce understanding.
- I now appreciate how layered encryption works — asymmetric for identity and key exchange, symmetric for speed.
- Definitely want to explore more about certificate chains and how browsers validate them.
