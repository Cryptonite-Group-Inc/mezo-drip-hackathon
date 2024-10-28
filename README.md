# Hackathon hosted by Mezo and Drip and in collaboration with Acre 🚀

Welcome to Hackathon hosted by Mezo and Drip and in collaboration with Acre! This repository serves as your central hub for all hackathon resources, demo implementations, and guidelines.

# DRIP Web3 Integration Hackathon

[Introduction placeholder]

## Demo Implementations 🛠️

### 1. [Discord Bot Demo](./discord-bot-demo)
A Discord bot demonstrating:
- Point balance checking
- User-to-user transfers

REPO: https://github.com/Cryptonite-Group-Inc/mezo-drip-hackaton-bot-demo

### 2. [Web Dashboard Demo](./web-dashboard-demo)
A Next.js web application showcasing:
- Real-time point tracking
- User search functionality
- Leaderboard visualization

REPO: https://github.com/Cryptonite-Group-Inc/mezo-drip-hackaton-web-demo

## Technical Documentation 📚

### DRIP API Resources
- [ReDoc Documentation](https://api.drip.re/redocs)
- [OpenAPI Documentation](https://api.drip.re/docs)
- [Extended API Guide](https://docs.drip.re/api/extended-api)

### Key API Features

#### Points Management
```typescript
// Get user points
GET /api/v4/realms/{realmId}/members/{userId}

// Transfer points
PATCH /api/v4/realms/{realmId}/members/{userId}/transfer
```

#### NFT Integration
```typescript
// Check NFT ownership
GET /api/v4/realms/{realmId}/web3/members/{userId}

// Setup NFT collection
POST /api/v4/realms/{realmId}/web3/collection/import
```

#### Leaderboard
```typescript
// Get realm leaderboard
GET /api/v4/realms/{realmId}/leaderboard
```

## Development Guidelines 💻

### Repository Structure
```
your-project/
├── README.md           # Project documentation
├── .gitignore        # Git ignore file
├── .env.example      # Example environment variables
└── src/              # Source code
```

### Essential Configuration Files

#### `.gitignore`
```
.env
.env.local
node_modules/
.DS_Store
```

#### `.env.example`
```
DRIP_API_KEY=your_api_key_here
DRIP_REALM_ID=your_realm_id_here
```

### Deployment Best Practices

1. **Environment Variables**
   - Never commit API keys
   - Use environment variables for configuration
   - Document all required variables

2. **Documentation Requirements**
   - Installation instructions
   - API integration examples
   - Configuration guide
   - Troubleshooting section

3. **Code Quality Standards**
   - TypeScript types inclusion
   - Consistent code style

### GitHub Repository Setup
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repo-name.git
git push -u origin main
```

## Technical Support Resources
- Developer Documentation: [docs.drip.re](https://docs.drip.re)
- Issue Reporting: [Create an issue](https://github.com/your-org/hackathon-repo/issues)
- API Status: [status.drip.re](https://status.drip.re)
