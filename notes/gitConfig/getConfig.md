## 🚀 Quick Start: Git Configuration
To ensure your contributions are attributed to the correct profile, verify your Git identity in Git Bash:

### Check Current Identity
```bash
# Check username
git config user.name

# Check email
git config user.email

# View all configurations
git config --list
```

# Global configuration (for all projects)
```bash
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
```
# Local configuration (for current repository only)
```bash
git config user.name "Project Alias"
git config user.email "alias@example.com"
```
