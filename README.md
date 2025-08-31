# Enterprise Case Studies — Security • Automation • Modernization • Healthcare

Short, anonymized write-ups of projects I’ve delivered. No proprietary code.

---

## 1) Security & Compliance (PCI-DSS)

**What I built**
- **RBAC for Admin Portal** — Permissions matrix (module/page/action), group profiles, and a management UI for Cloud Manager Portal (Both Admin and Customer Facing).
- **Duo Security MFA** — Push/SMS/Phone flow with a one-minute selection window; robust timeout/deny handling.
- **Inactive User Self-Reactivation** — PCI 90-day lockout → email passcode (5-min TTL) → secure reset.
- **Validation Framework Rebuild** — ParsleyJS-based validators across Network/Port/VPN/SSL-VPN.
- **Activity Logging** — who/what/when/outcome/reason; optimized list views for audits.

**Why it mattered**
- Reduced privileged-access risk, prevented silent failures, and improved auditability.
- Offloaded manual support actions with a secure self-service path.

**Stack**: Python/Django, Duo Security, ReactJS, ParsleyJS, SweetAlert2, DataTables

---

## 2) Infrastructure Automation (Nutanix Prism, Cisco FMC)

**What I built**
- **Nutanix v2 → v3 transition** — Modular Python wrappers, hybrid fallback, replication improvements; multi-cluster readiness via Prism Central.
- **Cisco FMC automation** — Port NAT/ACL lifecycle, enable/disable via ACL action; **S2S VPN** creation/edit/tunnels with safe deploys.
- **Register VM enhancement (solo)** — Added **registered-VM migration** between accounts with DC and pricing checks; automated order/billing.

**Why it mattered**
- Future-proofed platform against API deprecations and enabled multi-cluster scale.
- Standardized **port forwarding & S2S VPN** on **FTD-enabled VMs** via Cisco **FMC** APIs, with consistent NAT/ACL orchestration, idempotent updates, pre-deploy checks (deployable devices), and safe rollouts from a single Cloud Manager flow.
- Removed risky manual DB edits by automating order/billing during registered-VM migrations, eliminating billing/reporting drift.

**Stack**: Python, Django, Nutanix Prism APIs (v2/v3), Cisco FMC REST, JS ES6 + Promises, Docker

---

## 3) Healthcare SaaS

**What I built**
- Features for **EMR, lab reporting, appointment scheduling** in a **multi-tenant** cloud system.
- **Secure REST APIs** for interoperability (incl. SMS/device integrations) and **ReactJS/Redux** dashboards for clinician workflows.

**Why it mattered**
- Delivered real-world clinical features with security and compliance in mind.
- Improved practitioner UX (fewer clicks, consistent validation), enabling faster throughput.

**Stack**: Laravel/Yii (PHP), MySQL, ReactJS/Redux, jQuery/AJAX, Bootstrap, Git/Jira

---

## 4) Full-Stack Delivery & Leadership (Tecrux Global)

**What I did**
- Delivered **10+ full apps** (Laravel, ReactJS, modern JS) under tight deadlines; owned the **entire SDLC**.
- Integrated **PayPal, Stripe, Zoom, Google Maps, YouTube**; ran deployments and server ops (prod/stage).
- Rescued legacy stacks (Node.js, Magento, Babylon.js/Three.js) with little to no docs.
- Mentored **4+** juniors; task assignment, code reviews, onboarding.

**Why it mattered**
- Proved multi-hat leadership and delivery under pressure; reduced backlog and stabilized operations.

**Stack**: Laravel/PHP, ReactJS, ES6, MySQL/PostgreSQL/MongoDB, Node.js, WordPress

---

## 5) Supervisor Finder (FYP)

**What I did**
- Built a **Custom PHP MVC framework (from scratch)** — router via `.htaccess`, controllers/models/DAOs/views, form & request validators, clean separation of concerns, and secure session handling.
- **End-to-end platform** to match MS/PhD students with supervisors worldwide: search/filter (country, city, field), proposals, messaging, and admin moderation with **request triage** (accept/reject/waitlist/block).
- **Security-by-design:** tokenized email verification & password reset, hashed passwords, prepared statements, and front- & back-end validation with role-scoped access.

**Why it mattered**
- Replaced ad-hoc outreach with a **structured, auditable workflow** that reduces friction for students and supervisors.
- Demonstrated **full SDLC ownership** — requirements, use-case modeling, schema design, UI mockups, implementation, unit tests, and **complete documentation authored by me**.

**Stack**
PHP (custom MVC), MySQL, HTML/CSS/Bootstrap/JS/jQuery/AJAX, Apache + `.htaccess` routing

