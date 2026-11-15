# Awesome-Enterprise-Single-Sign-On-SSO
# Awesome-Enterprise-Single-Sign-On-SSO

## Top Enterprise Single Sign-On (SSO) Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on SAML 2.0 Federation, OIDC Providers & Self-Hosted Identity Platforms*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Single Sign-On (SSO)**. These tools help organizations centralize authentication across applications—covering everything from commercial IdP suites like Okta and Microsoft Entra ID to open-source identity providers that speak SAML 2.0, OIDC, and OAuth 2.0 without per-user licensing.

**Examples** include Okta, Microsoft Entra ID, OneLogin, PingFederate, CyberArk Identity, Google Workspace, Duo, Auth0, JumpCloud, Keycloak, and Authentik (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted SSO, open-source SAML/OIDC identity providers, and community-driven authentication platforms—ideal for organizations seeking data sovereignty and avoiding per-user SaaS pricing that compounds across workforces. The open-source landscape is anchored by **Keycloak**, the enterprise-grade standard backed by Red Hat and the CNCF, which includes SAML 2.0, OIDC, LDAP federation, and MFA with **no per-MAU fees** [citation:10].

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Okta](https://www.okta.com/)** | **The independent IAM benchmark.** Workforce Identity bundles SSO, MFA, and Universal Directory. **Starter: $6/user/month** (annual). **Essentials: $17/user/month** adds Adaptive MFA, Lifecycle Management, and Access Governance [citation:2]. **Single modules are no longer sold separately**—you buy a suite. A **$1,500/year minimum contract** applies to smaller teams [citation:12]. | Starter: **$6/user/month**; Essentials: **$17/user/month** | No free plan; annual billing only for workforce suites |
| **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)** | **The default for Microsoft estates.** SAML 2.0 and OIDC federation with Conditional Access. **P1: ~$7/user/month** standalone (list); **P2: ~$10/user/month** (list) [citation:13]. **Often bundled at no extra cost** with Microsoft 365 Business Premium, E3 (P1), or E5 (P2)—many organizations already own it [citation:3]. | P1: **~$7/user/month**; P2: **~$10/user/month** (standalone list) | **Free edition** included with Azure/M365; P1/P2 bundled in many enterprise plans |
| **[OneLogin](https://www.onelogin.com/)** | Mid-market SSO with SAML and OIDC. **Published tiers: Basic $3, Essentials $6, Business $10, Enterprise (quote)** per user/month [citation:4]. Vendr data shows buyers often achieve **$2.50–$5.00/user/month** for Advanced tier with annual prepayment. **Implementation adds $5K–$15K**; annual escalators of **3–5%** are common [citation:14]. | Basic: **$3/user/month**; Essentials: **$6**; Business: **$10** | Free trial available |
| **[CyberArk Identity](https://www.cyberark.com/)** | **Modular pricing with the lowest SSO entry point.** **Single Sign-On: $2/user/month**; Adaptive MFA: $3; Lifecycle Management: $4; Workforce Password Management: $5. **Real cost compounds**—SSO + MFA + Lifecycle = **~$9/user/month**, not $2 [citation:15]. | SSO: **$2/user/month**; Modules: $2–$5 each | No free tier; demo via sales |
| **[Google Workspace](https://workspace.google.com/)** | SAML-based SSO **included in all paid Workspace tiers**. **Business Starter: $7/user/month** (annual/fixed-term); Flexible plan: **$8.40/user/month** [citation:6]. **No free-seat allowance**—bills from seat 1. | Business Starter: **$7/user/month** (annual); Flexible: **$8.40** | **14-day free trial**; no permanent free tier |
| **[Duo](https://duo.com/editions-and-pricing)** | **Duo Free: $0 for 1–10 users**—genuine free tier for small teams. **Duo Essentials: $3/user/month** adds Single Sign-On (SAML/OIDC). Advantage ($6) and Premier ($9) add advanced access policies and reporting [citation:7]. | Free: **$0** (1–10 users); Essentials: **$3/user/month** | **Free forever**: 1–10 users, core MFA (SSO requires Essentials) |
| **[Auth0](https://auth0.com/pricing)** | Developer-first identity platform. **Free tier: 25,000 MAU**. **Self-Service SSO is available on select Enterprise plans only**—not on free or lower tiers. Dashboard SSO requires higher tiers [citation:8]. | Quote-only for SSO features; Free tier: 25K MAU | **Free**: 25,000 MAU (SSO not included); **Startup plan**: 100K MAU + SSO free for one year |
| **[JumpCloud](https://jumpcloud.com/)** | Cloud directory with SSO. **SSO package: ~$11/user/month** (annual listing)—positioned for organizations wanting directory + SSO + device management in one platform [citation:9]. | SSO: **~$11/user/month** | Free tier available for up to 10 users (limited features) |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Keycloak](https://github.com/keycloak/keycloak)** | [![Stars](https://img.shields.io/github/stars/keycloak/keycloak?style=social&color=white)](https://github.com/keycloak/keycloak/stargazers) | **The enterprise-grade open-source SSO standard.** Apache-2.0, backed by Red Hat and the CNCF. **SAML 2.0, OIDC, OAuth 2.0, LDAP/Active Directory federation, MFA, identity brokering, and fine-grained authorization**—all included with **no per-MAU fees and no feature gates** [citation:10]. **Realms provide multi-tenancy**. **Trade-off**: heavyweight deployment and a large configuration surface area—teams wanting quick setup may find initial configuration frustrating. **Best for enterprises needing battle-tested SSO** with deep customization and vendor-neutral open-source governance. |
| **[Authentik](https://github.com/goauthentik/authentik)** | [![Stars](https://img.shields.io/github/stars/goauthentik/authentik?style=social&color=white)](https://github.com/goauthentik/authentik/stargazers) | **The most approachable open-source SSO with the most flexible sign-in flows.** MIT core with paid enterprise features. **Flows and stages edited in the admin interface**—custom authentication logic without code. **The only leading open-source IdP with a SCIM provider** (push users to downstream apps). **Forward Auth** for Nginx-backed services is straightforward. **Best for teams with mixed technical backgrounds** wanting maintainable SSO without deep identity expertise. |
| **[Casdoor](https://github.com/casdoor/casdoor)** | [![Stars](https://img.shields.io/github/stars/casdoor/casdoor?style=social&color=white)](https://github.com/casdoor/casdoor/stargazers) | **Lightweight Go-based SSO with the widest protocol coverage.** Apache-2.0. **Single Go binary + React UI**—no JVM, no separate worker process. **SAML 2.0, OIDC, OAuth 2.0, CAS, LDAP, RADIUS, and SCIM** all supported. **Built-in MCP server with OAuth 2.1 for AI agents**. **70+ social/enterprise providers** including WeChat and DingTalk. **Syncers import users from Keycloak, Okta, Entra ID, and Google Workspace**—enabling gradual migration. **Best for teams wanting a lighter, UI-first IdP** with legacy protocol support and AI-agent readiness. |
| **[ZITADEL](https://github.com/zitadel/zitadel)** | [![Stars](https://img.shields.io/github/stars/zitadel/zitadel?style=social&color=white)](https://github.com/zitadel/zitadel/stargazers) | **Event-sourced SSO with the strongest audit trail and tenant isolation.** AGPL-3.0, Go/TypeScript. **SAML 2.0, OIDC, OAuth 2.0, and SCIM** support. **Instances → Organizations → Projects** hierarchy provides **infrastructure-level tenant isolation**. **Every mutation is an immutable event** for a complete, API-accessible audit trail. **API-first design** with connectRPC, gRPC, and REST. **Best for organizations needing the strongest audit trail and tenant isolation** with a modern API-first design. |
| **[Authelia](https://github.com/authelia/authelia)** | [![Stars](https://img.shields.io/github/stars/authelia/authelia?style=social&color=white)](https://github.com/authelia/authelia/stargazers) | **Lightweight SSO for protecting reverse proxy endpoints.** Go-based. **Not a standalone directory**—sits in front of Nginx, Traefik, or HAProxy and handles authentication and 2FA for services behind those proxies. **Best for homelabs and internal service protection** where a full IdP is overkill. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[WSO2 Identity Server](https://github.com/wso2/product-is)** | [![Stars](https://img.shields.io/github/stars/wso2/product-is?style=social&color=white)](https://github.com/wso2/product-is/stargazers) | **Open-source IAM with SAML, OIDC, OAuth2, SCIM 2.0, and FIDO2 support.** Apache-2.0. Recognized as a Digital Public Good by the Digital Public Goods Alliance. **Used in 93 countries** across finance, public administration, healthcare, and telecommunications. **Best for organizations wanting a recognized open-source IAM** with broad standards support and enterprise adoption. |
| **[Janssen Project](https://github.com/JanssenProject/jans)** | [![Stars](https://img.shields.io/github/stars/JanssenProject/jans?style=social&color=white)](https://github.com/JanssenProject/jans/stargazers) | **Linux Foundation-governed IAM server providing OAuth 2.0, OIDC, SAML, FIDO2/WebAuthn, and SCIM.** Apache-2.0. **Kubernetes-native with auto-scaling** for enterprise and national scale. **Low-code flow orchestration (Agama) and policy engine (Cedarling)** for custom authentication logic without forking the core. **Best for organizations needing population-scale SSO** with strong federation readiness. |
| **[Dex](https://github.com/dexidp/dex)** | [![Stars](https://img.shields.io/github/stars/dexidp/dex?style=social&color=white)](https://github.com/dexidp/dex/stargazers) | **OpenID Connect (OIDC) identity and OAuth 2.0 provider with pluggable connectors.** CNCF project. Often used as an authentication layer in Kubernetes clusters (integrates with Kubernetes API server OIDC). **Best for Kubernetes-native SSO** where Dex acts as the bridge between upstream IdPs and cluster authentication. |

**Frameworks for building custom systems**: Choose **Keycloak** for enterprise-grade SSO with the broadest protocol coverage and zero per-MAU fees [citation:10], **Authentik** for the most approachable setup with SCIM provisioning, **Casdoor** for a lightweight Go binary with built-in LDAP/RADIUS and AI-agent MCP support, or **ZITADEL** for event-sourced audit trails and strict tenant isolation —all without per-user pricing that compounds across large workforces.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- SSO platforms handle authentication credentials and identity data; enforce MFA, least-privilege access, and compliance with applicable regulations (GDPR, SOC 2, HIPAA where relevant). **A compromised IdP exposes every connected application.**
- **Commercial pricing has significant hidden costs and escalators.** **Okta** no longer sells SSO as a standalone module—Starter ($6/user/mo) bundles SSO+MFA+directory, but a **$1,500/year minimum** applies to smaller teams [citation:12]. **OneLogin's list prices** ($3–$10/user/mo) are starting points—implementation adds **$5K–$15K**, and annual escalators of **3–5%** are common [citation:14]. **CyberArk's $2/user/month SSO** looks cheapest but compounds to **~$9/month** when MFA and Lifecycle are added [citation:15]. **Duo offers a genuine free tier** for 1–10 users, but SSO requires the $3/user/month Essentials plan [citation:7]. **Auth0's self-service SSO is Enterprise-only**—the 25K MAU free tier does not include it [citation:8]. **Keycloak self-hosted has no per-MAU ceiling**—flat compute costs (~$10–20/month on Railway) versus Auth0's $2,000–$5,000/month at 50K MAU [citation:10]. **Validate whether SSO is already bundled in your existing Microsoft 365 or Google Workspace plan** before purchasing a standalone IdP—many organizations already own Entra ID P1/P2 through E3/E5 licensing [citation:3].

---

**Made for identity architects, IT administrators, and organizations building authentication infrastructure.**  
Let's make enterprise single sign-on more open, interoperable, and secure.
