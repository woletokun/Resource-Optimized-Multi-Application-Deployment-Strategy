# 🌐 Resource-Optimized Multi-Application Deployment Strategy  
### **Role:** DevOps Engineer / Cloud Infrastructure Engineer  
### **Server:** Hosted on (DigitalOcean)  
### **Technologies:** Laravel, MySQL, Nginx, Ubuntu, CI/CD, VTpass, Paystack, DigitalOcean Spaces  

---

## 🚀 Overview  
This project implements a **production-grade multi-application deployment** where three independent frontend applications:

- **App A → example.com**
- **App B → b.example.com**
- **App C → c.example.com**

all share:

✔ One Laravel backend  
✔ One MySQL database  
✔ One cloud server  
✔ One storage/CDN infrastructure  
✔ One fully automated CI/CD pipeline  

The goal was to deliver a **scalable, secure, optimized, and cost-efficient architecture** suitable for real-world production workloads.

---

## 🏗 Architecture Diagram

```
                +-------------------------------+
                |        Cloud Server           |
                |           Droplet             |
                +--------------------------------
                  |               |               |
         example.com         a.example.com   b.example.com
         (Frontend A)          (App B)         (App C)
                  \               |               /
                   \______________|______________/
                                  |
                     Laravel Backend API
                   /var/www/application-main
                                  |
                            MySQL Database
```

---

## ⚙ Key Deliverables

### 🔹 1. **Linux Server & Security Configuration**
- Hardened Ubuntu server
- UFW firewall rules
- Fail2Ban protection
- SSH key authentication
- System optimization (PHP-FPM, Nginx, MySQL)

---

### 🔹 2. **Nginx Multi-Domain Reverse Proxy**
Configured production-ready routing:

| Domain | Application |
|--------|-------------|
| example.com | App A |
| b.example.com | App B |
| c.example.com | App C |

All pointing to one backend:

```
https://example.com/api
```

Enabled:
- HTTP/2
- GZIP
- SSL (Certbot)
- Cache-Control
- SPA routing

---

### 🔹 3. **Laravel Backend Deployment**
- Composer install + production optimization
- `.env` configuration for all services
- Queue workers via Supervisor
- Cron scheduler
- Debugged VTpass MAC verification issue
- Redis queueing
- Optimized for high traffic

---

### 🔹 4. CI/CD Automation (GitHub Actions)
Pipeline handles:

- Build frontend assets
- Deploy backend & frontend
- Run migrations
- Clear caches
- Restart services
- Zero downtime deployment

---

### 🔹 5. Cloud Object Storage + CDN
Configured DigitalOcean Spaces with:

- CDN endpoint
- S3 filesystem driver  
- Secure access keys  
- High-performance asset delivery  

---

## 📊 Results
- **3 production apps** running on one backend  
- **Automated deployment workflow** implemented  
- **VTU, wallet, and payment systems live**  
- **Error-free callback signature validation**  
- **Scalable architecture ready for microservices**

---

## 🧠 Skills Demonstrated
- DevOps Engineering  
- Cloud Infrastructure  
- CI/CD Deployment  
- Linux Hardening  
- Laravel Backend Engineering  
- Nginx Reverse Proxy  
- API Integrations (Paystack, VTpass)  
- DigitalOcean Spaces (S3/CDN)  
- Production Debugging  
- High Availability Architecture  

---

## 📄 PDF Portfolio
A full PDF version of this project is available in this repo:

👉 [Download portfolio_project.pdf](./portfolio_project.pdf)

---

## 👤 Author  
**Oyewole Olatokun**  
DevOps Engineer • Cloud • Backend Infrastructure  
