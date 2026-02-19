# GitHub Pages Deployment Guide

This repository is configured to automatically deploy to GitHub Pages.

## What's Deployed

The `index.html` file serves as the landing page for this project on GitHub Pages. It contains:
- Project overview and description
- Features and capabilities
- Installation instructions
- FAQ section
- Download links to releases

## How It Works

The deployment is automated via GitHub Actions:
1. Any push to the `main` or `master` branch triggers the deployment workflow
2. The workflow can also be triggered manually via the Actions tab
3. The entire repository content is uploaded to GitHub Pages
4. The site becomes available at: `https://<username>.github.io/<repository-name>/`

## Repository Settings

To enable GitHub Pages for this repository:
1. Go to Repository Settings → Pages
2. Under "Build and deployment":
   - Source: Select "GitHub Actions"
3. The site will be published automatically on the next push

## Manual Deployment

To manually trigger a deployment:
1. Go to the Actions tab in the repository
2. Click on "Deploy to GitHub Pages" workflow
3. Click "Run workflow"
4. Select the branch and click "Run workflow"

## Local Testing

To test the landing page locally:
```bash
# Using Python 3
python3 -m http.server 8000

# Using PHP
php -S localhost:8000

# Using Node.js (with npx http-server)
npx http-server -p 8000
```

Then visit `http://localhost:8000` in your browser.

## Security Note

⚠️ **IMPORTANT**: The malicious build commands that were previously in the `.csproj` file have been removed. These commands attempted to download and execute code from external sources, which posed a serious security risk. The project is now safe to build and use.

## Support

For issues or questions, please use the [Issues](https://github.com/genXstark/Roobet-Crash-Predictor/issues) tab.
