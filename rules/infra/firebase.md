# Firebase & GCP

## Organization
- **Org**: agntc.tech (ID: 600894054507)
- **Owner**: justin@agntc.tech

## Projects
| Project | Purpose | URL |
|---------|---------|-----|
| power-to-the-people-vpp | Solar CRM | https://power-to-the-people-vpp.web.app |
| agentic-labs | Digital Justin, AI | https://agentic-labs.web.app |

## Test Credentials
- Email: `justin@agntc.tech`
- Password: `Solar2026!`

## Service Accounts
- MacBook: `~/Projects/power-to-the-people/firebase-service-account.json`
- Mac Studio: `/opt/digital-justin/firebase-service-account.json`

## Quick Commands
```bash
# Auth check
gcloud auth list
firebase login:list

# Deploy
firebase deploy --project power-to-the-people-vpp

# Enable service
gcloud services enable firestore.googleapis.com --project=PROJECT_ID
```

## Permissions (Full Access)
- Create/delete projects
- All Firebase services
- Firestore rules/indexes
- Auth users
- IAM roles

## Branch
| Need | See |
|------|-----|
| Firestore schema | @project-root/.claude/rules/firestore.md |
| Cloud Functions | @project-root/.claude/rules/functions.md |
