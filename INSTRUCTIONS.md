# Instructions for Publishing Your Privacy Policy

Follow these steps to publish your Privacy Policy to GitHub and use it for your SmartQR app on the Google Play Store.

## 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click on the "+" icon in the top-right corner and select "New repository"
3. Name your repository (e.g., "smartqr-privacy-policy")
4. Make it public
5. Add a description (optional)
6. Initialize with a README (optional)
7. Click "Create repository"

## 2. Upload the Privacy Policy Files

### Option 1: Upload through GitHub Web Interface

1. Navigate to your new repository
2. Click "Add file" > "Upload files"
3. Drag and drop or select ALL files from the PRIVACY_POLICY directory (make sure to include index.html)
4. Add a commit message (e.g., "Add privacy policy")
5. Click "Commit changes"

### Option 2: Upload via Git Command Line

```
cd PRIVACY_POLICY
git init
git add .
git commit -m "Add privacy policy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/smartqr-privacy-policy.git
git push -u origin main
```

## 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings"
3. In the left sidebar, click on "Pages" under "Code and automation"
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select "main" and "/(root)" folder
6. Click "Save"
7. Wait a few minutes for GitHub Pages to build your site

Your privacy policy will be available at: 
`https://YOUR_USERNAME.github.io/smartqr-privacy-policy/`

If you encounter a 404 error:
- Make sure you've uploaded the index.html file
- Double-check that GitHub Pages is properly configured
- Wait 5-10 minutes for the site to build
- Check the "Actions" tab to see if there are any deployment errors

## 4. Link the Privacy Policy in Google Play Console

1. Log in to your [Google Play Console](https://play.google.com/console/)
2. Select your SmartQR app
3. Go to "App content" in the left menu
4. Under "Privacy policy", click "Start" or "Edit"
5. Enter the URL to your privacy policy (use the GitHub Pages URL)
   - Example: `https://YOUR_USERNAME.github.io/smartqr-privacy-policy/`
6. Click "Save" and "Submit"

## 5. Update Your App Listing

If you're submitting a new app:
1. Complete all sections of your app listing
2. Make sure your app meets all Google Play policies
3. Submit for review

If you're updating an existing app:
1. Create a new release
2. Update your APK/AAB
3. Submit for review

## Note

If you make changes to your privacy policy in the future, make sure to:
1. Update the files in your GitHub repository
2. Update the "Last updated" date in the privacy policy files
3. Make sure your changes comply with Google Play policies 