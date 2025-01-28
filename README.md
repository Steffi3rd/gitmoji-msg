# Gitmoji-msg 💬
A simple utility to automatically add Gitmoji to commit messages based on their type using Husky.

## 🛠️ Installation

### Step 1: Install Husky
```bash
# Using Bun
bun add --dev husky

# Using pnpm
pnpm add --save-dev husky

# Using npm
npm install --save-dev husky
```

### Step 2: Initialize Husky
```bash
bunx husky init

pnpm exec husky init

npx husky init
```
The init command simplifies setting up husky in a project. It creates by default a `pre-commit` script in `.husky/` and updates the prepare script in `package.json`. Modifications can be made later to suit your workflow.

## 💬 Set Up Gitmoji-msg 

Move the file `prepare-commit-msg` to your `./husky` folder.


##  🚀 Usage
Now, whenever you make a commit, the script will automatically prepend a Gitmoji-msg to your commit message based on the type of commit.

For example:
- `feat: Add new feature` becomes `✨ feat: Add new feature`
- `fix: Fix bug` becomes `🐛 fix: Fix bug`

### 📋 Supported Gitmoji Types
- `✨ feat:` - New feature
- `🐛 fix:` - Bug fix
- `📝 docs:` - Documentation
- `💄 style:` - Style changes (e.g., CSS, indentation)
- `♻️ refactor:` - Code refactoring
- `✅ test:` - Tests
- `🔧 chore:` - Maintenance and chore tasks
- `⚡️ perf:` - Performance improvements
- `🚀 build:` - Build related changes
- `💚 ci:` - Continuous Integration
- `⏪️ revert:` - Reverting changes
- `🔥 remove:` - Removing code or files
- `📦️ package:` - Add or update dependencies
- `🚧 wip:` - Work in progress

## 🤝 Contributing
If you'd like to contribute in any way, please read our contribution guidelines and code of conduct.

## 📜 License
MIT License
