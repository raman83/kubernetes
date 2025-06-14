🧱 1. Built 3 Spring Boot Microservices
auth-service: OAuth2 token issuance with JWT and refresh tokens.

auth-switch-service: Validates client credentials and tokens.

gateway-service: Acts as an API gateway, forwarding requests and enforcing security.

🐳 2. Dockerized All Microservices
Dockerfiles and docker-compose.yaml to run all services locally.

Separate application.yaml profiles for local and prod.

🔐 3. Implemented OAuth2 With JWT
Issued access and refresh tokens using auth-service.

Configured auth-switch-service to validate access tokens.

Centralized token format and expiry management.

📦 4. Used Kubernetes for Deployment
Wrote Deployment, Service, and Ingress YAMLs for all services.

Applied ConfigMaps for environment-specific properties.

Used volumes to mount application-prod.yaml.

🌐 5. Set Up Ingress With TLS
Installed ingress-nginx via Helm.

Created and applied a TLS secret (mybank-tls).

Added DNS entry: local.mybank.com → 127.0.0.1

Verified HTTPS works using Postman: https://local.mybank.com/...

