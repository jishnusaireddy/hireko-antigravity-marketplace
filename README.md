# Hireko AI Recruiter — Google Antigravity Plugin

Official Antigravity plugin for **Hireko AI Recruiter**: candidate interview analytics, automated AI interview link generation, candidate match scorecards, and multi-tenant talent search.

---

## Capabilities

- 📊 **Candidate Pipeline & Analytics**: Fetch candidate counts, status breakdowns (completed vs. pending), and interview outcomes without leaving your chat.
- 🔗 **AI Interview Generation**: Create personalized interview links for candidates across all supported job funnels.
- 🎯 **Candidate Search & Scoring**: Retrieve semantic match scores and evaluation details for candidates evaluated by Hireko AI.
- 🔐 **Zero-Config Multi-Tenant Auth**: Direct local auth proxy (`bundle.mjs`) with seamless browser login. Recruiters simply enter their tenant credentials securely without manual key copying.

---

## Installation in Antigravity

### 1. From the Antigravity Marketplace (Recommended)
Search for **Hireko AI Recruiter** in Antigravity or ask in chat:
> *"Search marketplace for Hireko recruiter"*

Click **"Install"** on the plugin card:
```html
<plugin-card catalog-id="antigravity-plugins-partners/plugin/hireko-recruiter"></plugin-card>
```

### 2. From GitHub (CLI / Team Sharing)
Install directly using the Antigravity CLI:
```bash
agy plugin install https://github.com/jishnusaireddy/hireko-antigravity-marketplace
```

Or add to your project's `.agents/plugins.json`:
```json
{
  "inherits": [
    { "path": "https://github.com/jishnusaireddy/hireko-antigravity-marketplace" }
  ]
}
```

---

## Starter Prompts

Once installed, try asking:
- *"Show candidate interview counts and pass rates for my team"*
- *"Create a candidate interview link for Senior Backend Engineer"*
- *"Search candidates for Java Spring Boot and Microservices"*

---

## Engine & Architecture
- **Engine**: Local Stdio MCP Router (`node bundle.mjs serve`)
- **Downstream Tools**: 10 Recruiter Facade business tools
- **Authentication**: Multi-tenant AWS Cognito via browser device flow or direct credentials
