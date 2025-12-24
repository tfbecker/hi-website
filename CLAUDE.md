# Hi Website

Simple demo website deployed via Coolify to demonstrate the deployment workflow.

## Deployment Info

- **URL**: https://hi.becker.im
- **Repository**: https://github.com/tfbecker/hi-website
- **Coolify UUID**: `agcskw0kw8g0kcwo0g8c48co`
- **Build Pack**: Dockerfile
- **Port**: 80

## Stack

- nginx:alpine
- Static HTML/CSS

## Commands

```bash
# Restart
node ~/.claude/skills/coolify/scripts/deploy.js --restart agcskw0kw8g0kcwo0g8c48co

# View logs
node ~/.claude/skills/coolify/scripts/deploy.js --logs agcskw0kw8g0kcwo0g8c48co

# Check status
node ~/.claude/skills/coolify/scripts/deploy.js --app agcskw0kw8g0kcwo0g8c48co
```

## Updating

1. Make changes to files
2. Commit and push: `git add -A && git commit -m "message" && git push`
3. Coolify auto-deploys via webhook (or trigger manually with --deploy)
