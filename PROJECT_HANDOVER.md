# Sewota Etar - Project Handover & Status

**Date:** 2025-11-29
**Project ID:** `sewota-etar`

## 1. Project Goal
Duplicate the existing `firebaseEtar` project to create `sewotaEtar`, a localized version for the German company **Sewota**. This involves translating the interface to German, replacing branding (logos), and setting up a separate data environment.

## 2. Current Status
-   **Project Initialized:** The folder `/Users/attila/Dev/sewotaEtar` has been created.
-   **Git Initialized:** A local git repository has been initialized (`git init`).
-   **Firebase Configured:** The project is linked to the Firebase project `sewota-etar`.
-   **Analysis Complete:** We have identified the files requiring translation and the assets needing replacement.

## 3. Implementation Plan (To-Do)

### Localization
#### HTML Files (`public/`)
-   `index.html`: Marketing content, navigation, footer need translation to German.
-   `app.html`: App shell structure.
-   `privacy.html`: Needs a German version.

#### JavaScript Files (`public/js/`)
The following files contain hardcoded Hungarian strings that need to be translated:
-   `js/ui.js`: Login screens, dashboards, dynamic menus.
-   `js/partner.js`: Device list, tables, modals, filters.
-   `js/auth.js`, `js/admin.js`, `js/statistics.js`: Error messages, alerts.

#### Assets (`public/images/`)
-   Replace `ETAR_H.png`, `H-ITB_Logo.jpg`, `logo.jpg` with Sewota branding.

### Data Strategy
-   Decide whether to migrate existing data or start with a clean database.
-   Verify Firestore Security Rules for the new project.

## 4. How to Resume Work
1.  **Open the project** in your IDE.
2.  **Check `task.md`** (if available) or this file for the next steps.
3.  **Start Localization**: Begin translating the files listed above.
4.  **Deploy**: Use `firebase deploy` to test changes on the `sewota-etar` project.

## 5. Git Remote Setup (For moving to another machine)
To push this project to a remote repository (e.g., GitHub, GitLab), follow these steps:

1.  **Create a new empty repository** on your git provider (do not initialize with README/license).
2.  **Run the following commands** in this terminal:

```bash
# Add the remote repository (replace URL with your actual repo URL)
git remote add origin <YOUR_GIT_REPO_URL>

# Rename the branch to main (if not already)
git branch -M main

# Push the code
git push -u origin main
```

Once pushed, you can clone it on another machine using `git clone <YOUR_GIT_REPO_URL>`.
