# Azure Cloud Deployment — AI Chatbot Web App

This repository contains the AI chatbot web application deployed to **Microsoft Azure App Service** using **GitHub integration** (Deployment Center).  
The project demonstrates full cloud deployment, CI/CD automation via GitHub → Azure, and secure configuration using Azure RBAC and Managed Identity.

---

## 🚀 Azure Deployment Overview

### **App Service Deployment**
- **Platform:** Azure App Service (Node.js)
- **Deployment Method:** GitHub integration (automatic CI/CD via Deployment Center)
- **Runtime Stack:** Node.js 18 (Linux)
- **Public URL:** https://teams.microsoft.com/l/message/19:6145be23d476495c9ff7f70f1159faed@thread.v2/1763109173392?context=%7B%22contextType%22%3A%22chat%22%7D

### **Included Evidence**
- Screenshot of app running in the browser  
- Screenshot of Azure App Service dashboard  
- Screenshot of Deployment Center showing GitHub integration  
- Screenshot of successful deployment logs  

---

## 🔁 CI/CD Pipeline (GitHub → Azure)

The project uses Azure’s built-in Deployment Center:

### **How it works**
1. Code is pushed to the GitHub repo  
2. Azure automatically pulls the latest commit  
3. Azure performs:
   - Node.js install  
   - App build (if required)  
   - App Service deployment  
4. Azure restarts the app automatically

No manual ZIP uploads or manual builds were required.

---

## 🔐 Security / IAM

### Azure Identity & Access
- **Contributor role:** granted to allow resource creation & deployment  
- **Reader role:** used for monitoring  
- **App Service Managed Identity:** enabled for secure access to Azure resources  
- No secrets stored in code  
- Deployment was authenticated through GitHub OAuth

### Network Security
- HTTPS-only enabled  
- Public access allowed only for the web endpoint  
- SCM (deployment) endpoint protected by Azure authentication  

---

## ScreeenShots

### App Service overview



