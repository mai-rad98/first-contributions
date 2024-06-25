
```
# Hotfix for Production

When a critical issue is found in production, you need to apply a quick fix, known as a hotfix. 
This guide will walk you through the steps to create a hotfix, test it, and merge it back into both the production and development branches.

## Steps to Perform a Hotfix

### 1. Branch Off from Production/Main

First, you need to create a new branch from the `main` (or `production`) branch. This new branch is where you will make your hotfix changes.

**Command:**

```sh
git checkout main
git pull origin main  # Ensure you have the latest changes
git checkout -b hotfix/<hotfix-name>
```

Replace `<hotfix-name>` with a meaningful name for your hotfix.

### 2. Make Quick Fix and Commit

Next, you will make the necessary changes to fix the issue. Once the changes are made, you need to commit them.

**Commands:**

```sh
# Make your changes in your editor
git add .
git commit -m "Fix: <description of the fix>"
```

Replace `<description of the fix>` with a brief description of what you fixed.

### 3. Test Thoroughly

Before merging the hotfix, you need to test it thoroughly to ensure it resolves the issue and does not introduce new bugs. This step is crucial for maintaining production stability.

### 4. Merge Back to Production/Main and Development Branches

Once the hotfix has been tested and is confirmed to be working, you need to merge it back into both the `main` (production) and `develop` branches.
### 5. Clean Up

After the hotfix has been merged and pushed to both branches, you can delete the hotfix branch as it is no longer needed.

**Command:**

```sh
git branch -d hotfix/<hotfix-name>
git push origin --delete hotfix/<hotfix-name>
```
# Clean Up
``` sh
git branch -d hotfix/<hotfix-name>
git push origin --delete hotfix/<hotfix-name>
```
