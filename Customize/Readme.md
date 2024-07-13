

---

# Customization Guide for Daily Commit Automation

This guide provides step-by-step instructions on how to customize the Daily Commit Automation GitHub Actions workflow to suit your own GitHub account and repository.

## Prerequisites

Before proceeding with customization, ensure you have the following:

- Access to the GitHub repository where Daily Commit Automation is implemented.
- Basic knowledge of Git and GitHub Actions.
- Text editor of your choice for editing files.

## Steps for Customization

### 1. Fork the Repository

If you haven't already, fork the [Maintain-Streak](https://github.com/Yashasvi-30/Maintain-Streak) repository to your own GitHub account. This will allow you to make changes to the workflow files.

### 2. Clone the Repository

Clone your forked repository to your local machine using Git:

```bash
git clone https://github.com/your-username/Maintain-Streak.git
cd Maintain-Streak
```

Replace `your-username` with your actual GitHub username.

### 3. Navigate to the Workflow Directory

Navigate to the `.github/workflows` directory within your cloned repository. This directory contains the GitHub Actions workflow file (`daily-commit.yml`).

```bash
cd .github/workflows
```

### 4. Edit the Workflow File

Open the `daily-commit.yml` file in a text editor. This file contains the workflow definition in YAML format.

### 5. Modify Author Information

In the `daily-commit.yml` file, locate the `git config` commands where the author name (`Yashasvi Gupta`) and email address (`your-email@example.com`) are set. Modify these values to reflect your own GitHub username and email address.

Example:

```yaml
- name: Set author info
  run: |
    git config user.name "UserName"
    git config user.email "your-email@example.com"
```

Replace `"UserName"` with your GitHub username and `"your-email@example.com"` with your actual email address associated with GitHub.

### 6. Save the Changes

Save the `daily-commit.yml` file after making your modifications.

### 7. Commit and Push Changes

Commit the changes to your local repository and push them to GitHub:

```bash
git add daily-commit.yml
git commit -m "Customize GitHub Actions workflow for Daily Commit Automation"
git push origin main
```

### 8. Verify the Workflow

Navigate to the Actions tab in your GitHub repository. You should see that the workflow has been triggered. Check the workflow runs to ensure that commits are being made daily as expected.

### 9. Customize Commit Message (Optional)

If you want to customize the commit message that is committed daily, modify the `commit-message.txt` file located in the `daily-commits` directory. Edit the contents of this file to your liking.

### 10. Test the Automation

Create a new branch or make a change to trigger the workflow. Verify that daily commits are being made automatically with your customized author information.

## Additional Assistance

If you encounter any issues or have questions about customizing Daily Commit Automation, please refer to the [GitHub Issue Tracker](https://github.com/Yashasvi-30/Maintain-Streak/issues) for support.

---
