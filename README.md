# Reliable File Transfer Protocol using SSL (C)

## 📌 Overview
This project implements a reliable and secure file transfer system using:
- Sliding Window Protocol
- Packet Retransmission
- Timeout Handling
- SSL/TLS Encryption

---

## ⚙️ Features
- Secure communication using OpenSSL
- Sliding window (size = 4)
- Packet loss simulation
- Automatic retransmission
- Multi-client support

---

## 🧠 Concepts Used
- Computer Networks
- TCP Socket Programming
- Sliding Window Protocol
- SSL/TLS

---

## 📂 Project Files
- sender.c → Client
- receiver.c → Server
- cert.pem → SSL Certificate
- key.pem → Private Key

---

## 🖥️ Compilation

```bash
gcc sender.c -o sender -lssl -lcrypto
gcc receiver.c -o receiver -lpthread -lssl -lcrypto

▶️ Execution

Step 1: Run server

./receiver


Step 2: Run client

./sender
