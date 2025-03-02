## Steps to Set-up the project
node -v
npm -v
npx -v

npx create-next-app@15.0.3
cd .\google-docs-clone\
code .

npx shadcn@2.1.6 init
npx shadcn@2.1.6 add --all
npm run dev

## Initialize Git in Your Next.js Project
Step 1: Initialize Git
git init
Create a .gitignore file in the root directory and add the following:
node_modules/
.next/
.env
.DS_Store

Step 2: Set Up Your Remote Repository
git remote add origin https://github.com/your-username/your-repo.git

### Best Coding Practices for Git Commits & Repo Maintenance
Follow a Branching Strategy
git checkout -b feature/add-auth

Write Meaningful Commit Messages
feat: add user authentication
fix: resolve navbar styling issue
refactor: optimize API request logic
docs: update README with setup steps
chore: update dependencies

git add .
git commit -m "feat: implement user login functionality"

### Use Hooks to Enforce Code Standards
npx husky-init && npm install
npx husky set .husky/pre-commit "npm run lint && npm run test"

### Use Git Tags for Releases
git tag -a v1.0.0 -m "Initial release"
git push origin v1.0.0

Regularly Sync and Clean Up
git pull origin main
git branch -d feature/old-branch

### First Commit
git add .
git commit -m "chore: initialize Next.js project with Git"
#### Resolve ESLint warnings or errors
npm run lint
<!-- Add the below line to scripts in package.json -->
"test": "echo \"No tests configured\" && exit 0"

git push -u origin master

## Add Editor to the application
git checkout -b feature/add-editor

npm install @tiptap/react@2.10.2 @tiptap/pm@2.10.2 @tiptap/starter-kit@2.10.2 --legacy-peer-deps


