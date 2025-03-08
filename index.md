---
marp: true
---
<!-- _class: top -->

# OrgGuard – Automate GitHub Policy Checks & Visualize Compliance in Grafana
###### by Deexith Parandaman
<img src="https://raw.githubusercontent.com/deexithparand/cli-slides/main/jman_group_cover.webp" style="display: block; margin: auto;">

---

## About Me
###### (Just Another Developer)

<div style="display: flex; flex-direction: column; align-items: center; text-align: center; gap: 15px;">
  <div style="text-align: left; width: 100%;">
    - Platform Engineer at JMAN Group  <br>
    - Passionate about automation and DevOps  <br>
    - Loves building scalable and efficient solutions  
  </div>
  <img src="https://raw.githubusercontent.com/deexithparand/cli-slides/main/qr-code.png" style="max-width: 300px; display: block; margin: auto;">
</div>

---

## Motivation for OrgGuard
###### Why We Built This

- Managing GitHub user naming standards was difficult.
- Users had inconsistent names like **`ideexith`**, **`i_am_deexith`**, **`kickbuttowski`**.
- Unused invites occupied costly license spaces.
- No structured way to **audit** and **enforce policies**.
- **Solution:** Policy enforcement using **`OPA`**, **`Webhooks`**, and **`Grafana`**.

---

## Tech Flow
###### How OrgGuard Works

1. **GitHub Webhook** in Golang captures events.
2. **Ngrok** exposes local services for testing.
3. **Webhook Route** processes GitHub events.
4. **Triggers** on new member additions or invites.
5. **Sends Data to OPA** for policy validation.
6. **Stores Violations in PostgreSQL** for tracking.
7. **Visualizes Violations in Grafana** for insights.

---

## OrgGuard: The Setup
###### A Simple Yet Powerful Model

- **GitHub Webhooks** → **Golang Backend** → **OPA Policy Check**  
- **PostgreSQL** for storing violations  
- **Grafana Dashboard** for real-time insights  
- Deployable with **Docker Compose**  
- Supports **custom policies** for different organizations  

---
<!-- _class: title -->

## DEMO
###### Live Walkthrough of OrgGuard

---

## Why Self-Host OrgGuard?
###### Cost vs Buying GitHub Enterprise

- **GitHub Teams/Enterprise** is expensive.  
- **OrgGuard** offers custom policy enforcement at a lower cost.  
- **Greater flexibility** and **full control** over access rules.  
- **Audit logs and monitoring** without extra costs.  

---

## Extending OrgGuard
###### Possible Enhancements

- **Custom Webhook Actions** beyond user management.  
- **Enforce Repository Naming Conventions**.  
- **Track PR/Merge Commit Policies**.  
- **Implement Security Best Practices** like enforcing 2FA.  

---

## Thanks for Attending!
###### Reuse This Idea, Make It Better!

<div style="text-align: center;">
  <img src="https://raw.githubusercontent.com/deexithparand/cli-slides/main/thanks.gif" style="max-width: 300px; display: block; margin: auto;">
</div>
