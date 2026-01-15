# Setup Instructions

## Initialize Git Repository

```bash
cd /Users/marko/Code/agentify-test-pages
git init
git add .
git commit -m "Initial commit: Link checking test pages"
```

## Create New GitHub Repository

1. Go to GitHub and create a new repository (e.g., `agentify-link-checking-tests`)
2. **Don't** initialize it with README, .gitignore, or license
3. Copy the repository URL

## Push to GitHub

```bash
git remote add origin <your-github-repo-url>
git branch -M main
git push -u origin main
```

## Deploy to Vercel

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Import your new GitHub repository
4. **No build settings needed** - Vercel will serve the HTML files directly
5. Deploy

## Deploy to Netlify

1. Go to [netlify.com](https://netlify.com)
2. Click "Add new site" > "Import an existing project"
3. Connect your GitHub repository
4. **No build settings needed** - Netlify will serve the HTML files directly
5. Deploy

## Test Locally

```bash
# Python 3
python3 -m http.server 3000

# Or Node.js
npx http-server -p 3000
```

Then visit: http://localhost:3000/
