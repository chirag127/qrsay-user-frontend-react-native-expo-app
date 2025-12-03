# Contributing to ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App

We welcome and appreciate your contributions to **ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App**! This document outlines the guidelines and best practices for contributing to this Apex-grade mobile application. By following these guidelines, you help us maintain a high-quality, secure, and future-proof project.

## Table of Contents

1.  [Code of Conduct](#1-code-of-conduct)
2.  [How Can I Contribute?](#2-how-can-i-contribute)
    *   [Reporting Bugs](#reporting-bugs)
    *   [Suggesting Enhancements](#suggesting-enhancements)
    *   [Writing Code](#writing-code)
    *   [Improving Documentation](#improving-documentation)
3.  [Setting Up Your Development Environment](#3-setting-up-your-development-environment)
    *   [Prerequisites](#prerequisites)
    *   [Cloning the Repository](#cloning-the-repository)
    *   [Installing Dependencies](#installing-dependencies)
    *   [Running the Application](#running-the-application)
4.  [Development Workflow](#4-development-workflow)
    *   [Branching Strategy](#branching-strategy)
    *   [Commit Guidelines](#commit-guidelines)
    *   [Linting and Formatting](#linting-and-formatting)
    *   [Testing](#testing)
5.  [Architectural Principles](#5-architectural-principles)
6.  [Submitting Changes](#6-submitting-changes)
    *   [Pull Request Guidelines](#pull-request-guidelines)
    *   [Review Process](#review-process)
7.  [Security](#7-security)

---

## 1. Code of Conduct

This project adheres to a strict [Code of Conduct](https://github.com/chirag127/ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App/blob/main/CODE_OF_CONDUCT.md). Please ensure you read and follow it in all your interactions within this repository. We are committed to fostering an open and welcoming environment.

## 2. How Can I Contribute?

There are many ways to contribute, not just by writing code. Your participation, in any form, is highly valued.

### Reporting Bugs

If you find a bug, please open an issue using our [Bug Report template](https://github.com/chirag127/ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App/blob/main/.github/ISSUE_TEMPLATE/bug_report.md). Before submitting, please check existing issues to avoid duplicates. Provide detailed steps to reproduce the bug, expected behavior, and actual behavior. Screenshots or screen recordings are highly encouraged.

### Suggesting Enhancements

Do you have an idea for a new feature or an improvement to an existing one? Open an issue to discuss it. Clearly describe the enhancement, its potential benefits, and any design considerations. If it aligns with the project's vision, we can explore its implementation together.

### Writing Code

Ready to dive into the codebase? We welcome contributions of new features, bug fixes, and performance improvements. Please ensure your code adheres to our architectural principles and coding standards outlined below.

### Improving Documentation

Clear and comprehensive documentation is crucial. If you find gaps, inaccuracies, or areas for improvement in the `README.md`, comments, or any other documentation, your contributions are highly appreciated.

## 3. Setting Up Your Development Environment

To get started with development, follow these steps:

### Prerequisites

Ensure you have the following installed on your system:

*   **Node.js:** v18.x or higher (LTS recommended)
*   **npm:** v9.x or higher (comes with Node.js)
*   **Expo CLI:** `npm install -g expo-cli`
*   **Watchman:** Recommended for faster file system watching on macOS/Linux.

### Cloning the Repository

bash
git clone https://github.com/chirag127/ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App.git
cd ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App


### Installing Dependencies

bash
npm install


### Running the Application

To start the Expo development server:

bash
npm start


This will open a browser window with the Expo DevTools. You can then run the app on an iOS simulator, Android emulator, or your physical device using the Expo Go app.

## 4. Development Workflow

### Branching Strategy

We utilize a feature-branch workflow:

1.  **Main Branch:** `main` is the stable, deployable version. All pull requests are merged into `main` after review.
2.  **Feature Branches:** Create a new branch for each new feature, bug fix, or enhancement. Name your branches descriptively, e.g., `feat/add-qr-scanner`, `fix/login-bug`, `docs/update-readme`.

bash
git checkout main
git pull origin main
git checkout -b feat/your-feature-name


### Commit Guidelines

We enforce [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) to ensure a clear and consistent commit history. This helps with automatic changelog generation and semantic versioning.

*   **Format:** `<type>(<scope>): <description>`
    *   `type`: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`, `revert`
    *   `scope`: (Optional) The part of the codebase affected (e.g., `scanner`, `auth`, `ui`, `deps`)
    *   `description`: A concise summary of the changes.
*   **Example:** `feat(scanner): add real-time QR code detection`
*   **Breaking Changes:** Indicate breaking changes in the commit body with `BREAKING CHANGE: <description>`.

### Linting and Formatting

We use **Biome** for lightning-fast linting and formatting. Ensure your code adheres to the project's established style guides before submitting. You can run Biome to fix issues automatically:

bash
npx biome check --apply .
npx biome format --write .


Biome checks are integrated into our CI pipeline, so pull requests with linting or formatting errors will fail.

### Testing

All new features and bug fixes **must** be accompanied by appropriate unit and integration tests using **Jest**. Aim for high test coverage and ensure all existing tests pass.

bash
npm test


## 5. Architectural Principles

This project follows the **Feature-Sliced Design (FSD)** architecture for optimal scalability, maintainability, and clear separation of concerns. Adherence to principles like **SOLID**, **DRY (Don't Repeat Yourself)**, and **YAGNI (You Aren't Gonna Need It)** is also expected.

*   **SOLID Principles:** Ensure your code is Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion compliant.
*   **DRY:** Avoid code duplication. Abstract common logic into reusable components or modules.
*   **FSD:** Structure your code into `app`, `pages`, `widgets`, `features`, `entities`, `shared` layers for clarity and modularity.

## 6. Submitting Changes

### Pull Request Guidelines

Once your changes are ready, submit a Pull Request (PR) to the `main` branch. Use our [Pull Request Template](https://github.com/chirag127/ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App/blob/main/.github/PULL_REQUEST_TEMPLATE.md) to provide comprehensive details.

*   **One Feature/Fix Per PR:** Each PR should address a single, cohesive change.
*   **Descriptive Title:** A clear and concise title summarizing the PR's purpose.
*   **Detailed Description:** Explain *what* was changed, *why* it was changed, and *how* it was tested. Include screenshots or GIFs for UI changes.
*   **Link Issues:** Reference any related issues (e.g., `Closes #123`, `Fixes #456`).
*   **Pass CI/CD:** Ensure all automated checks (linting, testing, build) pass before requesting a review.

### Review Process

All pull requests require review by at least one maintainer. Expect constructive feedback and be prepared to iterate on your changes. Once approved, your PR will be merged into `main`.

## 7. Security

We prioritize security. When contributing, always consider potential security implications of your changes. Avoid hardcoding sensitive information, sanitize all user inputs, and adhere to secure coding practices. If you discover a security vulnerability, please report it privately as outlined in our [Security Policy](https://github.com/chirag127/ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App/blob/main/.github/SECURITY.md).

Thank you for contributing to ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App!