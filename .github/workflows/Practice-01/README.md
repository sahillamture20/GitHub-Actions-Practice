# GitHub Actions Practice - 01

A hands-on guide to creating and running your first GitHub Actions workflow. This project demonstrates the fundamentals of CI/CD automation using GitHub's native workflow system.

## 📋 Overview

This repository serves as a practical introduction to GitHub Actions, covering the essential steps needed to set up automated workflows. Whether you're looking to automate your development processes or streamline team collaboration, this guide provides a clear path forward.

## 🎯 What You'll Learn

- Creating a GitHub repository from scratch
- Setting up the `.github/workflows` directory structure
- Writing YAML workflow files
- Manually triggering workflows
- Viewing workflow logs and job execution details
- Understanding GitHub Actions terminology and concepts

## 🚀 Getting Started

### Prerequisites

- A GitHub account
- Basic understanding of Git and GitHub
- Familiarity with YAML syntax (helpful but not required)

### Step-by-Step Implementation

1. **Create a New Repository**
   - Navigate to your GitHub account
   - Click "New" to create a repository
   - Provide a repository name and optional description
   - Initialize the repository

2. **Set Up Workflow Directory**
   - Create a new file in your repository
   - Use the path: `.github/workflows/first-github-actions-practice.yml`
   - **Important**: GitHub only discovers workflows in the `.github/workflows` directory

3. **Write Your First Workflow**
   - Create a simple "Hello World" workflow
   - Define the workflow name, triggers, and jobs
   - Commit the changes

4. **Execute the Workflow**
   - Navigate to the "Actions" tab
   - Select your workflow
   - Click "Run workflow" to trigger manual execution
   - Monitor the workflow execution in real-time

5. **Review Workflow Logs**
   - Click on the workflow run to view detailed logs
   - Expand individual jobs to see step-by-step execution
   - Analyze the output and verify successful completion

## 📝 Workflow Configuration Example

```yaml
name: Day 01 - First GitHub Actions practice file

on:
  workflow_dispatch:

jobs:
  hello-world-job:
    runs-on: ubuntu-latest
    steps:
      - name: Print Hello World
        run: echo "Hello World from GitHub Actions!"
```

## 🔑 Key Concepts

- **Workflows**: Automated processes defined in YAML files
- **Jobs**: A set of steps that execute on the same runner
- **Steps**: Individual tasks within a job
- **Triggers**: Events that cause workflows to run (manual, push, pull request, etc.)
- **Runners**: Servers that execute your workflows

## 📂 Project Structure

```
.
├── .github/
│   └── workflows/
│       └── first-github-actions-practice.yml
└── README.md
```

## 🎓 Learning Outcomes

By completing this practice project, you will:

- Understand the basic structure of GitHub Actions workflows
- Know how to create and organize workflow files
- Be able to manually trigger and monitor workflows
- Have hands-on experience with CI/CD concepts
- Feel confident exploring more advanced GitHub Actions features

## 💡 Tips and Best Practices

- Always use descriptive names for workflows and jobs
- Add comments to your YAML files for clarity
- Start simple and gradually add complexity
- Review workflow logs to understand execution flow
- Use the Actions marketplace for pre-built actions
- Keep workflows focused on specific tasks

## 🤝 Contributing

Feel free to fork this repository and experiment with different workflow configurations. Share your learnings and improvements with the community!

## 📚 Resources

- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [Workflow Syntax Reference](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions)
- [GitHub Actions Marketplace](https://github.com/marketplace?type=actions)

## ✅ Completion Checklist

- [x] Repository created successfully
- [x] Workflow file structured correctly in `.github/workflows/`
- [x] First workflow written and committed
- [x] Workflow triggered manually via Actions tab
- [x] Workflow logs reviewed and verified
- [x] Understanding of basic GitHub Actions concepts achieved

---

**Congratulations!** You've successfully completed your first GitHub Actions workflow. This foundational knowledge will serve as a stepping stone for building more sophisticated automation pipelines.

## 📄 License

This project is open source and available for educational purposes.

---

*Made with ❤️ for the developer community*
