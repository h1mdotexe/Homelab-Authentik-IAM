I simply annoyed and tired of remembering all of my passwords for my growing applications. Instead of every application managing its own usernames and passwords. will act as your centralized authentication gateway and having my applications trust Authentik. 

Traffic Workflow:
Public Domian -> Cloudflare (DNS) -> Nginx Proxy Manager (NPM) -> Application

My NPM will act as my load balancer or intercept and route the authentication handshake to Authentik.

Project Success: 
Upon successful Multi-Factor Authentication (MFA), Authentik passes a secure cryptographic token (OIDC/SAML) back to grant access to internal services.
