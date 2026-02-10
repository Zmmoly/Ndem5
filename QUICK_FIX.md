# 🔥 Quick Fix - Build Failure

## The Problem
```
Execution failed for task ':app:processDebugGoogleServices'.
File google-services.json is not a valid JSON file.
```

## The 2-Minute Fix

### Step 1: Go to GitHub Secrets
- Your repo → **Settings** → **Secrets and variables** → **Actions**

### Step 2: Add Secret
- Click **"New repository secret"**
- Name: `GOOGLE_SERVICES_JSON`
- Value: Paste this (copy the entire block):

```json
{
  "project_info": {
    "project_number": "123456789000",
    "project_id": "nadeem-quran-app-test",
    "storage_bucket": "nadeem-quran-app-test.appspot.com"
  },
  "client": [
    {
      "client_info": {
        "mobilesdk_app_id": "1:123456789000:android:abcdef123456",
        "android_client_info": {
          "package_name": "awab.quran.ar"
        }
      },
      "oauth_client": [
        {
          "client_id": "123456789000-abcdefghijklmnop.apps.googleusercontent.com",
          "client_type": 3
        }
      ],
      "api_key": [
        {
          "current_key": "AIzaSyDEMO_KEY_FOR_TESTING_ONLY"
        }
      ],
      "services": {
        "appinvite_service": {
          "other_platform_oauth_client": [
            {
              "client_id": "123456789000-abcdefghijklmnop.apps.googleusercontent.com",
              "client_type": 3
            }
          ]
        }
      }
    }
  ],
  "configuration_version": "1"
}
```

### Step 3: Rebuild
- Go to **Actions** tab
- Find your failed build
- Click **"Re-run failed jobs"**

## ✅ Done!
Your build should now succeed.

---

## Better Solution (Optional)

Replace your workflow file with the improved version that auto-generates valid mock configs:

1. Copy `android-build-IMPROVED.yml` 
2. Save it as `.github/workflows/android-build.yml` in your repo
3. This will work even without the secret (generates valid mock config automatically)

---

## For Production

When you're ready for production:
1. Get real `google-services.json` from [Firebase Console](https://console.firebase.google.com/)
2. Replace the GitHub secret with real Firebase config
3. Firebase Auth, Firestore, Storage will work in the app

---

**That's it!** The mock config lets you build and test, real config enables Firebase features.
