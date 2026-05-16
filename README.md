<img width="3000" height="859" alt="image" src="https://github.com/user-attachments/assets/bfc53f63-e52a-46f3-9b2c-573da2996b86" />


I simply was annoyed and tired of remembering all of my passwords for my growing applications list😅. Instead of every application managing its own usernames and passwords. This will act as my centralized authentication gateway and having my applications trust Authentik. 

Traffic Workflow:
Public Domian -> Cloudflare (DNS) -> Nginx Proxy Manager (NPM) -> Application

My NPM will act as my load balancer or intercept and route the authentication handshake to Authentik.

Project Success: 
Upon successful Multi-Factor Authentication (MFA), Authentik passes a secure cryptographic token (OIDC/SAML) back to grant access to internal services.
