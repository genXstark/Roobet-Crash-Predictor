# Enabling GitHub Pages - Step by Step

To complete the deployment of this repository to GitHub Pages, follow these steps:

## Prerequisites
- You must have admin access to this repository

## Steps to Enable GitHub Pages

1. **Navigate to Repository Settings**
   - Go to your repository: `https://github.com/genXstark/Roobet-Crash-Predictor`
   - Click on the "Settings" tab (requires admin access)

2. **Access Pages Settings**
   - In the left sidebar, click on "Pages" (under "Code and automation")

3. **Configure Build and Deployment**
   - Under "Build and deployment" section:
     - **Source**: Select "GitHub Actions" from the dropdown
     - This will enable the workflow we've created (`.github/workflows/deploy.yml`)

4. **Save and Wait**
   - The settings are saved automatically
   - GitHub Actions will automatically deploy the site
   - The first deployment may take 1-2 minutes

5. **View Your Site**
   - Once deployed, your site will be available at:
     - `https://genxstark.github.io/Roobet-Crash-Predictor/`
   - The URL will also be shown in the Pages settings page

## Manual Deployment (Optional)

If you want to trigger a manual deployment:

1. Go to the "Actions" tab in your repository
2. Click on "Deploy to GitHub Pages" workflow in the left sidebar
3. Click "Run workflow" button on the right
4. Select the branch (main/master) and click "Run workflow"

## Verifying the Deployment

After enabling GitHub Pages:

1. Check the "Actions" tab to see if the workflow ran successfully
2. Look for a green checkmark next to the latest workflow run
3. Click on the workflow run to see details and logs
4. Visit your GitHub Pages URL to confirm the site is live

## Troubleshooting

If the deployment fails:

1. Check the workflow logs in the Actions tab
2. Ensure the repository is public (or you have GitHub Pro/Enterprise for private repo Pages)
3. Verify that GitHub Actions is enabled for your repository
4. Check that the workflow file exists at `.github/workflows/deploy.yml`

## After Deployment

Once your site is live:
- Any push to the main/master branch will automatically redeploy the site
- Changes typically appear within 1-2 minutes
- You can view deployment history in the Actions tab

## Need Help?

If you encounter any issues:
- Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
- Review workflow logs in the Actions tab
- Open an issue in this repository for support
