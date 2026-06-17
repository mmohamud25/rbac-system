# RBAC System — Role-Based Access Control

A browser-based Identity and Access Management (IAM) project built as a hands-on portfolio demonstration of core RBAC principles. No backend. No frameworks. Pure HTML, CSS, and JavaScript with localStorage persistence.

**Live Demo:** [rbac-system.mmohamud.me](https://rbac-system.mmohamud.me)

---

## What It Does

This project simulates a real-world access control environment where an administrator can manage users, define roles, assign granular permissions, visualize the access matrix, and run live access simulations — all with a full audit trail.

### Features

| Module | Description |
|---|---|
| Dashboard | Live stats: total users, roles, permissions, audit events |
| User Management | Create, deactivate, and remove users; assign roles |
| Role Management | Define roles and attach permissions to each |
| Permissions | Create granular permissions by resource and action type |
| Access Matrix | Visual grid mapping every role to its permissions |
| Simulate Access | Real-time check: can this user perform this action? |
| Audit Log | Timestamped record of every identity and access change |

---

## IAM Concepts Demonstrated

- **Role-Based Access Control (RBAC)** — users inherit permissions through roles, not direct assignment
- **Principle of Least Privilege** — roles only hold the permissions they need
- **Identity Lifecycle** — create, activate, deactivate, and remove users
- **Access Simulation** — enforce policy checks at runtime based on role membership
- **Audit and Compliance** — every change is logged with timestamp and action type
- **Separation of Duties** — roles like Auditor vs Admin have non-overlapping permission sets

---

## Default Data

The system seeds with four roles and eight permissions out of the box so you can explore immediately:

**Roles:**
- Admin — full system access
- SOC Analyst — alert triage and IOC management
- Viewer — read-only across all resources
- Auditor — logs, reports, and compliance read access

**Permissions include:** `alerts:read`, `alerts:write`, `users:admin`, `logs:read`, `reports:export`, `ioc:read`, `ioc:write`, `config:admin`

---

## Tech Stack

- Vanilla HTML, CSS, JavaScript
- localStorage for data persistence (no backend required)
- Google Fonts: Playfair Display, DM Sans, JetBrains Mono
- Deployed via GitHub Pages

---

## How to Run Locally

```bash
git clone https://github.com/mmohamud25/rbac-system.git
cd rbac-system
open index.html
```

No install. No build step. Open the file and it works.

---

## Deploying to GitHub Pages

1. Push `index.html` to your repo's `main` branch
2. Go to **Settings > Pages**
3. Set source to `main` branch, root folder
4. Your site will be live at `https://yourusername.github.io/rbac-system`

To use a custom subdomain, add a `CNAME` file containing your subdomain (e.g. `rbac-system.mmohamud.me`) and configure your DNS accordingly.

---

## Project Context

This is part of a broader IAM portfolio built to demonstrate hands-on access control knowledge alongside certifications including CompTIA Security+ (SY0-701) and ISC2 Certified in Cybersecurity (CC).

Planned follow-up projects:
- Identity Governance Dashboard (access request and approval workflows)
- OAuth 2.0 / OIDC SSO Demo
- Zero Trust access model with policy engine

---

## Author

**Mohamed Mohamud**
Founder, Kulan Group | Cybersecurity & Technology
[mmohamud.me](https://mmohamud.me) · [linkedin.com/in/mohamed-2-mohamud](https://linkedin.com/in/mohamed-2-mohamud)
