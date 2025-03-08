---
marp: true
---
<!-- _class: top -->

# OrgGuard: Enforcing GitHub Policies with OPA
###### by Deexith Parandaman
---

## About Me
###### (Just Another Developer)
- Platform Engineer at JMAN Group
- Passionate about automation and DevOps
- Loves building scalable and efficient solutions

![JMAN Group Logo](https://x.com/JMANGroup/header_photo)

---

## Motivation for OrgGuard
###### Why We Built This
- Managing GitHub user naming standards was a mess.
- Users had inconsistent names like `ideexith`, `i_am_deexith`, `kickbuttowski`.
- Unused invites consumed costly license spaces.
- No easy way to automate audits and enforce policies.
- **Solution**: Policy enforcement on GitHub using **OPA + Webhooks + Grafana**.

---

## Tech Flow
###### How OrgGuard Works
1. **GitHub Webhook in Golang**
2. **Ngrok** for exposing local services
3. **Webhook Route** for handling GitHub events
4. **Trigger on Member Add/Invite**
5. **Send Data to OPA for Policy Validation**
6. **Store Violations in PostgreSQL**
7. **Visualize Everything on Grafana**

---

## OrgGuard: The Setup
###### A Simple Yet Powerful Model
- GitHub Webhooks → Golang Backend → OPA Policy Check → PostgreSQL → Grafana Dashboard
- Deployable with **Docker Compose**
- Supports **custom policies** for different orgs

---
<!-- _class: title -->

## DEMO
###### Live Walkthrough of OrgGuard

---

## Why Self-Host OrgGuard?
###### Cost vs Buying GitHub Enterprise
- **GitHub Teams/Enterprise** is expensive.
- **OrgGuard** provides custom policy control at a fraction of the cost.
- **More flexibility** and **full control** over policy enforcement.
- **Audit logs and monitoring** without extra cost.

---

## Extending OrgGuard
###### What You Can Do
- **Custom Webhook Actions** beyond user management.
- **Enforce Repository Naming Conventions**.
- **Track PR/Merge Commit Policies**.
- **Enforce 2FA & Security Best Practices**.

---

## Thanks for Attending!
###### Reuse This Idea, Make It Better!

![Thanks](https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZWFyc2dyN3l1cWFlZmhzY3RqbDh0eWFsc2VyZjl4dXF5NnM2cGNnYiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/KJ1f5iTl4Oo7u/giphy.gif)

### 📩 Connect with Me

![Contact QR](qr-code.png)

