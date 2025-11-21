# Deployment Guide for Vercel

## Option 1: Deploy via Vercel CLI (Recommended)

### Step 1: Login to Vercel
```bash
vercel login
```
This will open a browser window. Follow the instructions to authenticate.

### Step 2: Deploy
```bash
vercel
```
Follow the prompts:
- Set up and deploy? **Yes**
- Which scope? Select your account
- Link to existing project? **No** (for first deployment)
- Project name? **pushyati** (or your preferred name)
- Directory? **./** (current directory)
- Override settings? **No**

### Step 3: Deploy to Production
```bash
vercel --prod
```

## Option 2: Deploy via GitHub Integration (Easier)

1. Go to [vercel.com](https://vercel.com)
2. Sign up/Login with your GitHub account
3. Click "Add New Project"
4. Import your repository: `ramniks05/pushyati`
5. Select the branch: `feature/product-data-management` (or merge to main first)
6. Vercel will auto-detect settings
7. Click "Deploy"

## Option 3: Deploy via Vercel Dashboard

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Drag and drop your project folder
4. Click "Deploy"

## Important Notes

- The `vercel.json` file is already configured
- Your JSON data file will be accessible at: `https://your-domain.vercel.app/data/products.json`
- All HTML files will work correctly
- The site will be live at: `https://your-project-name.vercel.app`

## After Deployment

Your site will be live at a URL like:
- `https://pushyati.vercel.app`
- Or a custom domain if configured

Test the product pages:
- `https://your-domain.vercel.app/products.html`
- `https://your-domain.vercel.app/products.html?category=nutraceuticals`

