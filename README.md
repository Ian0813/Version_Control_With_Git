# Coursera - Version Control With Git Final Project

This project is designed to simulate team collaboration and the release production process using Git branching strategies. The goal is to demonstrate how multiple team members can work on different features, bug fixes, or tasks simultaneously while managing releases across different branches.

## Certificate Link

[Version Control with Git Certificate - Ian Chen](https://coursera.org/share/121a13b3d69affb514249a29d62fbb56)

## Project Overview

In this repository, you will find the simulation of a typical team workflow using Git.

- Multiple branches for different stages of development (feature branches, release branches, and production).
- A series of commits representing team members working on separate tasks.
- A simulated release process with version tags applied on specific branches.

The project will demonstrate how to:

- Use Git for parallel development by utilizing different branches for feature development, bug fixes, and production releases.
- Manage releases by creating and tagging versions.
- Merge work from different branches while resolving conflicts.
- Simulate the deployment process with different versions of the product.

## Branching Strategy

This repository uses a standard branching strategy that can be customized for team workflows.

The key branches involved are:

- `master`: The master production branch where the final, stable version of the product is always available.
- `develop`: The development branch where all features are integrated before being released.
- `feature/{feature-name}`: Feature branches where individual tasks or new features are developed.
- `release1/{version}`: Release branches for preparing production-ready versions of the software.
- `hotfix1/{fix-name}`: Hotfix branches for quick fixes on production issues.

## Workflow Overview

1. **Feature Development**:
   - Developers create a new `feature` branch off of `develop` to work on new features.
   - Once the feature is complete, a pull request (PR) is made to merge the feature into the `develop` branch.

2. **Release Preparation**:
   - When `develop` is ready for a new release, a release branch is created from `develop`.
   - Final touches, bug fixes, and optimizations are applied on the release branch.
   - After all changes are reviewed and tested, the release branch is merged into `master` and tagged with the version number (e.g., `v1.00`).

3. **Production Release**:
   - The `master` branch always reflects the stable version of the application.
   - The production code is deployed from the `master` branch.

4. **Hotfixes**:
   - If a critical issue arises in production, a hotfix1 branch is created from `master` to address the issue immediately.
   - After the hotfix1 is complete, it is merged back into both `master` and `develop`.

## Getting Started

To get an overview of the git workflow in this repository, please follow the steps below.

### 1. Clone the repository
```bash
git clone https://github.com/Ian0813/Version_Control_With_Git.git

```
### 2. Display the commit history with a graph representation
```bash
git log --graph --online --all
