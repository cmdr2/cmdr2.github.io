---
title: "GitHub Actions Wizard released!"
date: 2025-09-10T10:13:31
slug: "github-actions-wizard-released-ci-deployment"
tags:
  - github
  - actions-wizard
  - ci
  - cd
---

# GitHub Actions Wizard released!

Wrote [GitHub Actions Wizard](https://github.com/cmdr2/github-actions-wizard) to make it easier to setup CI on my projects (especially new ones). More details from the project page:

"""

**GitHub Actions Wizard** is a simple tool for generating GitHub Actions workflows for common deployment tasks.

Built primarily for my needs, but you're free to use it, if you find it useful.

It goes beyond simple workflow generation by automatically setting up necessary permissions (such as creating AWS IAM Roles and Policies for S3 or Lambda deployments). The intent is to quickly generate the overall workflow boilerplate, and then customize by editing the generated file.

To use it, run the `github-actions-wizard` CLI tool in your repository's folder, and answer the interactive prompts. The generated workflow file will be saved in your repository's `.github/workflows` folder. You can customize the file further, as necessary.

"""

It currently supports the following Workflow Templates:
- **Python package** - build and publish to PyPI
- **npm package** - build and publish to npm
- **Static Hugo website** - build and deploy to GitHub Pages
- **Static S3 website** - build and deploy to AWS S3
- **Static Cloudflare Pages website** - build and deploy to Cloudflare Pages
- **AWS Lambda** - build and deploy to AWS Lambda
- **itch.io** - build and publish to itch.io
- **Pytest CI** - run tests with pytest on push and pull request (test-only)
- **Custom workflow**