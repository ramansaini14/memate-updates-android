📋 Overview
This repo serves as the distribution point for compiled JavaScript bundles that can be delivered directly to your mobile app. The bundles here are designed to work with the react-native-ota-hot-update library.

🚀 Purpose
Store production-ready JS bundles for different app versions

Manage multiple deployment environments (Staging, Production)

Track bundle versions and update metadata

Serve as the source for OTA update delivery

📦 Available Bundles
Bundles are organized by platform and environment:

Production Bundles
iOS: ios/production/[version].bundle

Android: android/production/[version].bundle

Staging Bundles
iOS: ios/staging/[version].bundle

Android: android/staging/[version].bundle

🔄 Update Process
Bundle Creation: New bundles are built from the main React Native codebase

Versioning: Each bundle follows semantic versioning (e.g., 1.2.3)

Deployment: Bundles are uploaded to this repository

Distribution: The app checks this repository for available updates

Application: Updates are downloaded and applied automatically

📝 Update Metadata
Each bundle is accompanied by a metadata file that includes:

Version number

Release notes

Compatibility information

Checksum for verification

Release date

⚠️ Important Notes
Native Code Changes: Updates to native code still require app store submissions

Compatibility: Bundles must match the native app version

Testing: All bundles are tested in staging before production deployment

Rollback: Previous versions are maintained for emergency rollbacks

🔒 Security
All bundles are served over HTTPS

Checksum verification ensures bundle integrity

Access controls limit who can upload new bundles

📊 Version History
See the readme.md file for detailed version history and release notes for each bundle version.

🆘 Support
If you encounter issues with a specific bundle version:

Check the version compatibility with your app

Verify the bundle checksum matches the metadata

Roll back to a previous stable version if needed

Note: This repository contains only compiled JavaScript bundles. The source React Native code is maintained in a separate repository.

