---
layout: default
title: Privacy policy — Erebus Trial 2 Sync
---

# Privacy policy

Erebus Trial 2 Sync is a single-user file-copy automation operated by its account owner. This policy describes the application's configured behavior once authorization and setup are complete.

## Access and use

The application requests Google Drive access so it can work with existing destination files. The OAuth permission covers Drive more broadly than the destination folder. The workflow is configured to copy files only into the selected destination folder.

The workflow uses destination file and folder metadata and checksums to identify, update, and verify copied files. It copies committed source files from the owner's GitHub repository into Google Drive. Source-repository deletions do not automatically delete destination copies. A later run can overwrite changes made directly to a copied destination file.

## Processing and sharing

The automation runs on GitHub Actions and uses Google's Drive API through rclone. Google and GitHub process the data needed to provide those services under their respective terms and privacy policies.

The copy workflow does not sell Google user data, use it for advertising, or transmit it to AI services for inference or model training. Its intended use follows the Google API Services User Data Policy, including the Limited Use requirements.

This documentation website has no application analytics, advertising scripts, or credential-entry forms. Its hosting provider may process normal web-request information under its own policies.

## Storage and retention

Authorization credentials are stored in a GitHub Actions repository secret and written into a temporary runner configuration for each authorized job. The workflow includes cleanup of that temporary configuration. The repository secret remains until the owner removes or replaces it.

Copied files remain in Google Drive until the owner removes them. Workflow logs may contain file paths, transfer details, and errors, and remain subject to the repository's GitHub Actions log-retention settings. This tool does not create a separate application database.

## Control and revocation

The account owner can disable the workflow in GitHub Actions, remove its repository secret, and revoke the application's Google account authorization. Revoking access stops future authorized transfers; it does not remove copies already stored in Drive or existing GitHub workflow logs. The owner manages those copies and logs separately.

## Contact

Use the application support address displayed on the Google authorization screen.

[Application home page](index.html)
