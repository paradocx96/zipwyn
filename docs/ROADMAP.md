## Roadmap

**Delivered**

- [x] Serverless redirect backend defined as code
- [x] Multi-stage deploys and custom domains
- [x] Hardened headers, validation and rate limiting
- [x] Git-driven web deployments on Vercel

**Planned - platform & DevOps**

- [ ] GitHub Actions CI for lint, type-check and build on every pull request
- [ ] GitHub Actions CD for the serverless stack using AWS OIDC (no long-lived keys)
- [ ] Replace static AWS keys in the web app with short-lived credentials (Vercel OIDC → IAM role)
- [ ] Define all DynamoDB tables and indexes in one IaC stack, shared by both apps
- [ ] CloudWatch alarms and dashboards (5xx, throttles, latency); structured logging
- [ ] Custom domain and ACM certificate managed as code
- [ ] Per-function least-privilege IAM and AWS WAF on the HTTP API
- [ ] Distributed rate limiting (the current limiter is in-memory per instance)
- [ ] Docker Compose with DynamoDB Local for one-command local development
- [ ] Automated tests (validation unit tests, API integration tests)

**Planned - product**

- [ ] Billing and plan quota enforcement
- [ ] Link expiration, bulk creation and richer analytics (referrers, geography, devices)
