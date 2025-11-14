# Azure IAM Policy Summary

## Assigned Roles
### 1. Contributor (Primary deployment role)
- Allows creating, editing, and deploying Azure resources  
- Required for connecting GitHub Deployment Center  
- Needed to restart App Service, view deployment logs, and configure settings  

### 2. Reader (Monitoring role)
- Allows viewing logs, health status, and metrics  
- Useful during debugging & verification  

---

## App Service Authentication & Identity
### System-Assigned Managed Identity
- Turned on in App Service  
- Enables future secure access to Azure Key Vault, Storage, etc.  
- No credentials stored in code  

---

## Security Principles Used
- Least privilege access  
- Role-based access control (RBAC)  
- HTTPS enforcement  

---

## Notes
All deployments were performed using authenticated GitHub integration, meaning no secrets or tokens were manually stored.
