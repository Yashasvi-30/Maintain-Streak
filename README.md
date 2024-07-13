# Daily Commit Automation with GitHub Actions

**Headline:**  
Effortlessly maintain your GitHub streak with automated daily commits.

## Objective
The objective of this project is to provide a GitHub Action that automates the process of making daily commits. By creating a new text file each day in a designated folder, this workflow helps developers maintain their GitHub streak effortlessly.

## Project Structure

### 1. .github/workflows
This directory contains the GitHub Actions workflow files. These YAML files define the automated processes and tasks that GitHub will execute. The `daily-commit.yml` workflow schedules a daily job to create and commit a new text file with the current date and time.

### 2. README.md
The `README.md` file provides a comprehensive overview of the project. It includes the purpose, setup instructions, usage guidelines, and details on how to customize the workflow to suit individual needs.

### 3. daily_commits
The `daily_commits` folder is where the daily text files are created and stored. Each file is named with the current date and contains the author name, username, and commit timestamp. This ensures a new file is added to the folder every day, keeping your GitHub activity consistent.

### 4. Customize
The `Customize` section includes a guide on how to personalize the GitHub Actions workflow. It provides step-by-step instructions on how to modify the `daily-commit.yml` file to match your own GitHub account details and preferences. This ensures that the automation works seamlessly for any user.

### 5. Contributions
Contributions are welcome! Other developers can access this repository, review the workflow, suggest improvements, and contribute to the project. This section outlines the guidelines for contributing, including how to fork the repository, make changes, and submit pull requests.

### 6. SRS (Software Requirements Specification)
The SRS document provides a detailed technical specification for the project. It includes the requirements, functionalities, and constraints of the GitHub Actions workflow. This document serves as a reference for developers looking to understand the technical aspects and requirements of the automation process.

---

## Detailed Working

### How It Works
1. **Triggering the Workflow**:
   - The GitHub Actions workflow is scheduled to run daily at a specified time. The schedule is defined using cron syntax in the `daily-commit.yml` file.

2. **Generating the File**:
   - Each day, the workflow generates a new text file within the `daily_commits` directory. The file is named with the current date and contains the following information:
     - Author name: Yashasvi Gupta
     - Username: Yashasvi-30
     - Commit timestamp

3. **Committing the File**:
   - After generating the file, the workflow commits it to the repository with a commit message that includes the current date and time.

4. **Maintaining the Streak**:
   - By ensuring a new file is committed to the repository each day, the workflow helps maintain an active GitHub streak, showcasing consistent activity.

### Key Components
- **GitHub Actions Workflow**:
  - The core of the automation is the GitHub Actions workflow defined in `.github/workflows/daily-commit.yml`.
  - It uses the following key actions:
    - `actions/checkout@v2`: Checks out the repository.
    - `actions/setup-node@v2`: Sets up the Node.js environment.
    - `actions/commit@v2`: Commits the new file to the repository.

- **Scheduled Cron Job**:
  - The workflow uses a cron schedule to trigger the daily job. This ensures the automation runs at the same time each day, maintaining consistency.

---


## Detailed Description

### .github/workflows
- **Purpose**: Contains the GitHub Actions workflow definition.
- **Key File**: `daily-commit.yml`
  - **Description**: This workflow file schedules a job to run daily at a specified time. The job creates a new text file in the `daily_commits` directory with the current date and time, then commits this file to the repository.

### README.md
- **Purpose**: Provides a comprehensive overview of the project.
- **Contents**:
  - Project objective and structure.
  - Setup and customization instructions.
  - Contribution guidelines.

### daily_commits
- **Purpose**: Stores the daily created text files.
- **Contents**: Each file is named with the current date and includes:
  - Author name: Yashasvi Gupta
  - Username: Yashasvi-30
  - Commit timestamp

### Customize
- **Purpose**: Guide for personalizing the GitHub Actions workflow.
- **Steps**:
  1. **Edit Workflow File**: Modify `.github/workflows/daily-commit.yml` to customize author details and commit messages.
  2. **Personalize the README**: Update the `README.md` with your own instructions and project details.
  3. **Adapt to Your Needs**: Make any other necessary changes to fit your specific use case and preferences.

### Contributions
- **Purpose**: Encourage and guide community contributions.
- **Guidelines**:
  1. Fork the repository.
  2. Create a new branch for your feature or bugfix.
  3. Make your changes and ensure they are well-tested.
  4. Submit a pull request with a detailed description of your changes.

### SRS (Software Requirements Specification)
- **Purpose**: Provide a detailed technical specification for the project.
- **Contents**: Includes requirements, functionalities, and constraints of the GitHub Actions workflow.

---
