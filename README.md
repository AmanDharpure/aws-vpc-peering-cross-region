# aws-vpc-peering-cross-region
AWS Project demonstrating cross-region VPC Peering between Singapore and Mumbai with EC2 private connectivity.
# 🌐 AWS Cross-Region VPC Peering Project

This project demonstrates how to establish **private connectivity between two AWS VPCs across different regions** using VPC Peering.

---

## 🚀 Project Overview

- Region 1: Singapore
- Region 2: Mumbai (ap-south-1)
- Goal: Enable EC2 instances to communicate using **Private IP**

---

## ⚙️ Services Used

- AWS VPC
- EC2 (Windows Server)
- Internet Gateway
- Route Tables
- Security Groups
- VPC Peering

---

## 🔧 Steps Summary

### 1. Create VPC in Singapore
- CIDR: 10.0.0.0/16
- Subnet: 10.0.0.0/24

### 2. Create VPC in Mumbai
- CIDR: 192.168.0.0/16
- Subnet: 192.168.0.0/24

### 3. Configure Networking
- Attach Internet Gateway
- Update Route Tables
- Configure Security Groups (ICMP, RDP, SSH)

### 4. Launch EC2 Instances

### 5. Test Connectivity
❌ Initial ping failed (no peering)

### 6. Setup VPC Peering
- Create cross-region peering connection
- Accept request
- Update routes in both VPCs

### 7. Final Result
✅ Successful ping using Private IP

---

## 📚 Key Learnings

- VPCs are isolated by default
- Peering enables private communication
- Route tables are crucial
- Security groups must allow ICMP

---

## 💡 Future Improvements

- Implement AWS Transit Gateway
- Add Load Balancer
- Hybrid Cloud setup

---

## 👨‍💻 Author

Aman Dharpure

---

## ⭐ If you found this useful, give it a star!
