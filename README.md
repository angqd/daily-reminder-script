# Daily Reminder Email Script

This repository contains a Python script that sends a daily reminder email at 11:30 AM UTC using GitHub Actions.

## Setup Instructions

1. Fork this repository to your GitHub account

2. Set up the following secrets in your repository:
   - Go to Settings > Secrets and variables > Actions
   - Add the following secrets:
     - `SENDER_EMAIL`: Your Gmail address
     - `SENDER_PASSWORD`: Your Gmail app password (see note below)
     - `RECIPIENT_EMAIL`: Your girlfriend's email address

3. Enable GitHub Actions:
   - Go to the Actions tab
   - Enable workflows for this repository

## Important Notes

### Gmail App Password
To use Gmail as the sender, you'll need to:
1. Enable 2-Step Verification on your Google Account
2. Generate an App Password:
   - Go to Google Account settings
   - Security
   - 2-Step Verification
   - App passwords
   - Generate a new app password for "Mail"

### Time Zone
The script runs at 11:30 AM UTC. Make sure to adjust the time in the GitHub Actions workflow file if you need a different time zone.

## Testing
You can manually trigger the workflow from the Actions tab to test if everything is working correctly. 