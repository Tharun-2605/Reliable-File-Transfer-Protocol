# Reliable File Transfer Protocol using SSL (C)

## Overview
This project implements a reliable file transfer system using:
- Sliding Window Protocol
- Timeout & Retransmission
- SSL/TLS Security

---

## Features
- Secure file transfer using OpenSSL
- Sliding window (size = 4)
- Packet loss simulation
- Retransmission of lost packets
- Multi-client support

---

## Files
- sender.c → Client side
- receiver.c → Server side

---

## Compilation

gcc sender.c -o sender -lssl -lcrypto
gcc receiver.c -o receiver -lpthread -lssl -lcrypto

---

## Execution

Step 1: Run server
./receiver

Step 2: Run client
./sender

---

## Working

1. File split into packets
2. Each packet assigned sequence number
3. Sender sends packets in window
4. Receiver sends ACK
5. Lost packets retransmitted

---

## Packet Loss Simulation
Every 3rd packet is dropped once to test reliability.

---

## Security
Uses SSL/TLS encryption via OpenSSL.

---

## Author
Your Name
