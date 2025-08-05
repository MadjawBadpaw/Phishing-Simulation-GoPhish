# Phishing-Simulation-GoPhish
A phishing simulation project using GoPhish and MailHog to demonstrate how phishing campaigns work in a safe, isolated environment. Includes fake landing pages, email templates, and campaign analytics to train and test user awareness—designed for educational and SOC analyst learning purposes.
# 🎯 Phishing Simulation with GoPhish & MailHog  

A safe phishing simulation project using **GoPhish** and **MailHog**, built to demonstrate phishing campaign workflows, credential capture, and reporting in a controlled lab environment. Designed for SOC analyst training, ethical hacking labs, and awareness testing.

---

## 📌 Objectives
- Simulate phishing attacks safely in a local environment.
- Create realistic phishing landing pages (e.g., Office 365).
- Track email opens, link clicks, and credential submissions.
- Generate reports to analyze user behavior and improve awareness.

---

## 🛠 Tools Used
- **[GoPhish](https://github.com/gophish/gophish)** – Open-source phishing framework.
- **[MailHog](https://github.com/mailhog/MailHog)** – Local email testing server.
- **Kali Purple** (or any Linux environment).
- **HTML/CSS** – For phishing page customization.

---

## 🔧 Setup & Workflow
1. **Install GoPhish** and **MailHog** locally.  
2. Configure MailHog SMTP (`127.0.0.1:1025`) as GoPhish sending profile.  
3. Create:
   - Phishing **landing page** (with data capture).
   - Phishing **email template** with `{{.URL}}`.
   - Fake **user group** (dummy emails).
4. Launch a test campaign:
   - Send phishing emails (captured in MailHog).
   - Click links → Submit fake credentials.
5. Analyze results in GoPhish Dashboard (open %, click %, data captured).  

---

## 📊 Campaign Results

| Metric                | Value        |
|---------------------- |------------- |
| Total Emails Sent     | 5            |
| Opened Emails         | 2            |
| Clicked Links         | 2            |
| Submitted Credentials | 1            |
| Email reported        | 2            |


---


## 🛣 Roadmap
- [x] Set up GoPhish & MailHog in isolated lab.
- [x] Create phishing landing page (365 style).
- [x] Launch campaign with dummy users.
- [x] Capture and analyze results.
- [ ] Automate PDF report generation.
- [ ] Add user-awareness redirect page.
- [ ] Test with public SMTP relay (future scope).

---

