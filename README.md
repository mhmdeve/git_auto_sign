# Git Commit Message "Signed-off-by" Hook

## Overview

This Git repository includes a custom Git hook that automatically adds a "Signed-off-by" line to your commit messages. The "Signed-off-by" line indicates that you have read and agreed to the [Developer's Certificate of Origin (DCO)](https://developercertificate.org/). Adding this line is a common practice in open-source projects.

## How it Works

When you make a commit or cherry-pick a commit, this Git hook checks if your commit message already contains a "Signed-off-by" line. If it doesn't, the hook appends a "Signed-off-by" line with your name and email, as configured in your Git settings.

## Installation

To install this hook in your Git repository, follow these steps:

1. Navigate to your Git repository's `.git/hooks` directory.

2. Create a new file named `commit-msg` if it doesn't already exist.

3. Make the `commit-msg` file executable by running the following command:

   ```bash
   chmod +x commit-msg
## Configuration
Before using this hook, make sure your Git username and email are correctly configured. You can set them using the following Git commands:

    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    
## Usage
After you've installed the Git hook, you don't need to do anything extra. When you make a new commit or cherry-pick a commit, the hook will automatically add the "Signed-off-by" line to your commit message if it's not already there.