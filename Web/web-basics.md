---

# 🌐 Web Basics

The web is a global network that allows users to access and share information through websites, applications, and online services.

This document covers the foundational concepts needed to understand how the web works.

---

## 🧩 What is the Web?

The web is built on three core ideas:

- **Clients** → Users or browsers that request information  
- **Servers** → Machines that store and send data  
- **Networks** → The connection between them

The browser sends a request → the server responds → content is displayed.

---

## 🔑 Key Components

### 🖥 Web Browser
Used to access websites  
Examples: Chrome, Firefox, Safari, Edge

### 🗄 Web Server
Hosts websites and handles requests  
Examples: Apache, Nginx, IIS

### 🔐 Protocols
Control how data is transferred

- **HTTP** — Unencrypted communication
- **HTTPS** — Secure & encrypted communication (TLS/SSL)

---

## 🧱 Website Structure

### 🎨 Frontend (Client-Side)
Runs in the browser

- HTML — Structure
- CSS — Styling
- JavaScript — Interactivity

### ⚙️ Backend (Server-Side)
Handles logic and data

- Databases
- APIs
- Authentication
- Business logic

---

## 🔗 Request–Response Cycle (Simplified)

1️. User enters a URL  
2️. Browser sends a request  
3️. Server processes it  
4️. Server returns a response  
5️. Browser displays the page

This is the foundation of how web apps work.

---

## 🚀 Recommended Learning Path (Coming Soon)

These topics will be added as separate files:

- HTML Basics — `html-basics.md`
- CSS Basics — `css-basics.md`
- JavaScript Basics — `js-basics.md`

---

## 💡 Tips for Beginners

- Build small projects (portfolio, blog, landing page)
- Experiment in browser DevTools
- Practice writing clean HTML & CSS
- Learn how requests & responses work

---

📌 *Section below explains domains & DNS as part of Web & Cybersecurity fundamentals.*

---

## 🌍 Domain Names & DNS

A domain name is a human-readable address that maps to an IP address (example: `google.com`).

DNS (Domain Name System) works like the **phonebook of the internet** — it translates domain names into IP addresses.

---

## 🏷 Types of Domains

### 🔸 Top-Level Domains (TLDs)

These are the highest level in the domain hierarchy.

Examples:

- `.com`
- `.org`
- `.net`
- `.edu`
- `.gov`

---

### 🌎 Country Code TLDs (ccTLDs)

Used for specific countries or regions:

- `.pl` — Poland  
- `.in` — India  
- `.uk` — United Kingdom  
- `.de` — Germany  

Sometimes used for branding (example: `.io`, `.ai`).

---

### 🧩 Generic TLDs (gTLDs)

Industry / purpose-based domains:

- `.tech`
- `.dev`
- `.app`
- `.store`
- `.cloud`

Widely used in startups & projects.

---

### 🏠 Second-Level Domain (SLD)

This is the main domain name:

Example:

- In `example.com`
  - `example` → Second-level domain
  - `.com` → TLD

---

### 🔹 Subdomains

A sub-section of a domain:

Examples:

- `blog.example.com`
- `api.example.com`
- `support.example.com`

Subdomains are commonly used for:

- apps
- services
- testing environments

---

## 🧠 How DNS Works (Simple Flow)

1️⃣ User enters a domain → `example.com`  
2️⃣ Browser asks DNS resolver  
3️⃣ DNS finds the IP address  
4️⃣ Browser connects to the server  
5️⃣ Website loads

---

## 🧾 Common DNS Records

| Record | Purpose |
|-------|--------|
| A | Maps domain → IPv4 address |
| AAAA | Maps domain → IPv6 address |
| CNAME | Alias to another domain |
| MX | Mail server records |
| TXT | Text / verification data |
| NS | Nameserver for domain |
| PTR | Reverse DNS lookup |
| SOA | Domain authority + metadata |

---

### 🔍 Examples

A record:

```text
example.com → 142.251.42.78
```

CNAME:

```text
www.example.com → example.com
```

MX record:

```text
example.com → mail.example.com
```

TXT record (used for verification):

```text
Google-Site-Verification=....
```

---

## 🔐 Why DNS is Important in Security

DNS is critical for:

- phishing detection
- domain spoofing analysis
- traffic monitoring
- incident response

Security tools often inspect:

- DNS logs
- suspicious domains
- redirect chains

---

📌 *This file is part of my learning roadmap for Web & Cybersecurity fundamentals.*
