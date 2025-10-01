# Concept of Bug Bounty, Scope, Public vs Private
A bug Bounty is a program that is offered by organisations ( companies , government , agencies ) that allows hackers to legally find and report security vulnerabilities , bugs , and flaws in their systems, applications, or website. In return, these organisations provide recognition and , most importantly , financial compensations ( the “bounty” ) for valid and impactful findings.

# Scope -

In bug bounty scope is the clearly defines set of rules, assets, and boundaries that an organization provides for its bug bounty programs. 

  1. In scope ( allowed to Test ) - The specific applications, domains, IP ranges, feature, or any 

technologies that hackers are permitted to test for vulnerabilities.

1. Out of scope ( Not allowed to Test ) - Assets, actions, or vulnerability types that are explicitly forbidden. Testing these could lead to legal issues or no reward. 

# Public and Private Programs

### Public Programs

Public Programs are open to anyone. they typically listed on platforms like Hackerone, Bugcrowd or multiple other platforms any registered hacker can view the program details, scope, and start hunting for bugs.

Pros for Hackers:

1. Accessibility to anyone
2. learning opportunities for Beginners
3. Volume of Targets
4. Reputation Building
5. Work from anywhere

## Private Programs

Private bug bounty programs are invite only. Companies hand-pick group of trusted often highly skilled, security researchers from  a platform’s talent pool to participate. These programs are not visible to general public on the platforms. 

Pros for Hackers:

1. Less competition
2. Higher Payouts
3. Access to Sensitive Target
4. Direct communication with Organizations
5. Contract Based Penetration Testing

# **Skills required for Bug Bounty**

## 1. Foundational technical skills (must-have)

These are the baseline things you must understand.

### 1.1 Web fundamentals

**Definition:** How websites and web apps work (HTTP, cookies, sessions, HTML, JavaScript).

**Why it matters:** Most bounties are web-app bugs (XSS, CSRF, SQLi, auth flaws).

**Key subskills:**

- HTTP request/response lifecycle (methods, headers, status codes).
- HTML & DOM basics (how pages render, where inputs live).
- JavaScript basics (DOM manipulation, client-side logic).
- Cookies, localStorage, session management.
    
    **Practice:** Inspect network tab, read raw HTTP, build a simple HTML/JS page.
    

### 1.2 Networking basics

**Definition:** How computers communicate over the internet (DNS, TCP/IP, TLS).

**Why it matters:** Understanding endpoints, ports, and secure channels helps with recon and exploitation.

**Key subskills:** DNS lookup, ports, TLS/HTTPS basics, basic packet flow.

**Practice:** Use `ping`, `dig`/`nslookup`, `telnet`/`nc` to connect to services.

### 1.3 Operating systems & command line

**Definition:** Comfortable using Linux/Windows and terminal commands.

**Why it matters:** Many tools run in terminals; payload crafting and exploitation often require OS-level knowledge.

**Key subskills:** File system, permissions, `curl`, `wget`, `ssh`, `grep`, `sed`, `awk`.

**Practice:** Set up a Linux VM and navigate tasks in the terminal.

### 1.4 Programming / scripting

**Definition:** Ability to read and write small scripts to automate tasks and create PoCs.

**Why it matters:** Automating recon, crafting payloads, and writing repeatable PoCs is essential.

**Recommended languages:** Python (easy, many libs), JavaScript (for client-side PoCs), Bash.

**Key subskills:** HTTP requests, parsing responses (JSON/XML), basic regex.

**Practice:** Write a Python script that requests an API and parses JSON.

## 2. Security Knowledge for Bug Bounty

### 2.1 Web Application Vulnerabilities

- SQL Injection (SQLi)
- Cross-Site Scripting (XSS) → Reflected, Stored, DOM
- Cross-Site Request Forgery (CSRF)
- Broken Authentication (weak login, session fixation)
- Broken Access Control (IDOR, privilege escalation)
- Security Misconfigurations (default creds, directory listing)
- Server-Side Request Forgery (SSRF)
- Remote Code Execution (RCE)
- Local File Inclusion (LFI) / Remote File Inclusion (RFI)
- Path Traversal (Directory Traversal)
- Open Redirects
- Clickjacking
- File Upload Vulnerabilities
- Insecure Deserialization
- Sensitive Data Exposure (unencrypted data, hardcoded secrets)
- XML External Entity (XXE)
- Command Injection

---

### 2.2 API & Mobile Security

- CORS Misconfiguration
- JWT / OAuth / SAML Token Attacks
- Rate Limiting & Brute-Force Bypass
- Broken Object-Level Authorization (BOLA)
- Excessive Data Exposure
- GraphQL-Specific Issues (introspection, nested queries)
- Insecure Direct API Access
- Mobile App Flaws (insecure storage, exposed API keys)

---

### 2.3 Business Logic & Advanced Bugs

- Business Logic Flaws (workflow bypass, price manipulation)
- Race Conditions (double-spending, concurrent requests)
- Mass Assignment (modifying hidden parameters)
- Privilege Escalation via Logic Flaws
- Password Reset Flaws (token reuse, predictable reset links)
- Account Takeover Techniques (session hijacking, weak reset flows)

---

### 2.4 Infrastructure & Cloud Security

- Cloud Misconfigurations (AWS S3, GCP buckets, Azure blobs)
- Exposed Services (Elasticsearch, Redis, MongoDB)
- Subdomain Takeover
- SSRF → Cloud Metadata Extraction
- Misconfigured CI/CD Pipelines
- Exposed Secrets in Code (GitHub, config files)

---

### 2.5 Other Key Areas

- Information Disclosure (debug pages, stack traces, .git folders)
- Cryptographic Flaws (weak hashing, hardcoded keys, SSL/TLS issues)
- Insecure Caching
- Logic Bypass in Payment Systems (coupon abuse, price manipulation)
- Supply Chain Issues (dependency confusion, npm/PyPI attacks)

## Top Platforms for Bug Bounty

- **HackerOne** — largest marketplace; great for beginners (Hacker101). https://www.hackerone.com
- **Bugcrowd** — strong community + training (Bugcrowd University). [https://www.bugcrowd.com](https://www.bugcrowd.com/?utm_source=chatgpt.com)
- **Synack (SRT)** — invite-only, high value, for experienced testers. https://www.synack.com/red-team
- **Intigriti** — EU-focused, regular challenges, beginner-friendly. https://www.intigriti.com
- **YesWeHack** — GDPR-friendly European platform. https://www.yeswehack.com
- **Open Bug Bounty** — open disclosure, easy to start (lower payouts). https://www.openbugbounty.org
- **SafeHats** — India / APAC regional platform. https://www.safehats.com
- **Zerocopter** — invite/private programs for experienced hunters. https://www.zerocopter.com
