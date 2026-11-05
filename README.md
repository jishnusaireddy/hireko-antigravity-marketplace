# Hireko Antigravity Marketplace

Official Antigravity marketplace repository for Hireko AI Recruiter tools and plugins.

## Included Plugins

| Plugin | Category | Description |
| :--- | :--- | :--- |
| **Hireko AI Recruiter** (`hireko-recruiter`) | Productivity | Candidate interview analytics, AI interview links, and search scorecards. |

## How to Install in Antigravity

### Method 1: Local / User Config (All Workspaces)
Extract the `hireko-recruiter` folder into:
`~/.gemini/config/plugins/hireko-recruiter`

### Method 2: Shared Git Project
Add to your project's `.agents/plugins.json`:
```json
{
  "inherits": [
    { "path": "https://github.com/jishnusaireddy/hireko-antigravity-marketplace" }
  ]
}
```
