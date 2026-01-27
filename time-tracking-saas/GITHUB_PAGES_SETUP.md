# GitHub Pages Setup Guide

## Quick Fix Checklist

### 1. Verify Repository Structure
Your repository on GitHub should have this structure:
```
time-tracking-saas/          (repository root)
├── index.html              ← Must be at root
├── .nojekyll               ← Already created
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
├── about.html
├── contact.html
└── ... (all other HTML files)
```

**IMPORTANT:** If your files are inside a `time-tracking-saas` subdirectory on GitHub, move them to the repository root!

### 2. GitHub Pages Configuration
1. Go to your repository: `https://github.com/srivathsan999/time-tracking-saas`
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under **Source**, select:
   - Branch: `main` (or `master` if that's your default branch)
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for GitHub to build your site

### 3. Verify Repository Name
- Repository must be named exactly: `time-tracking-saas`
- Repository must be **Public** (or you have GitHub Pro)
- Your username: `srivathsan999`

### 4. Check Branch Name
- Default branch should be `main` or `master`
- All files must be committed and pushed to this branch

### 5. Verify Files Are Committed
Run these commands in your repository:
```bash
git status
git add .
git commit -m "Fix GitHub Pages setup"
git push origin main
```

### 6. Test the URL
After configuration, test:
- `https://srivathsan999.github.io/time-tracking-saas/`
- `https://srivathsan999.github.io/time-tracking-saas/index.html`

Both should work.

## Common Issues

### Issue: 404 Error
**Solution:** 
- Ensure `index.html` is in the repository root (not in a subdirectory)
- Check GitHub Pages is enabled in Settings → Pages
- Verify the branch name matches your default branch

### Issue: Styles/Images Not Loading
**Solution:**
- All paths are relative (already correct: `assets/css/style.css`)
- Ensure all files are committed and pushed

### Issue: Still Getting 404 After Setup
**Solution:**
1. Go to repository Settings → Pages
2. Click "Save" again (even if already saved)
3. Wait 5-10 minutes for GitHub to rebuild
4. Clear browser cache and try again

## Verification Steps

1. ✅ `.nojekyll` file exists (prevents Jekyll processing)
2. ✅ `index.html` is in repository root
3. ✅ All assets folder is committed
4. ✅ GitHub Pages is enabled in Settings
5. ✅ Branch is set to `main` or `master`
6. ✅ Repository is public

## Still Not Working?

If you're still getting 404:
1. Check the repository URL: `https://github.com/srivathsan999/time-tracking-saas`
2. Verify files are visible in the repository root on GitHub
3. Check the Actions tab for any build errors
4. Try accessing: `https://srivathsan999.github.io/time-tracking-saas/index.html` directly

