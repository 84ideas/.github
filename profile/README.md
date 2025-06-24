# 🏢 Organization Repository

[![Board Status](https://dev.azure.com/OhMyMood/7ff679aa-e0bd-4882-870c-e451d3626bc8/01d4841c-4b08-4020-b868-c13d1db3583f/_apis/work/boardbadge/cc301ffa-bb4d-4e9a-848d-fa00e1a873f9)](https://dev.azure.com/OhMyMood/7ff679aa-e0bd-4882-870c-e451d3626bc8/_boards/board/t/01d4841c-4b08-4020-b868-c13d1db3583f/Stories/)

Welcome to the **84ideas** repository! This serves as the central hub for our projects, documentation, and resources.

## 📌 Repos


# Team Structure & Workflow

### 1. Overview

This document outlines the new team structure and workflow setup for this project, including how we will utilize GitHub and Azure DevOps in our daily operations.

---

### 2. Team Structure

- **Maris**: Focus on business side of Swoep Focus on business side of Swoep
- **Musa**: Works on Swoep back-end development / Project Manager — contact for task-related questions
- **Mason**: Works on Swoep back-end development
- ???

---

### 3. GitHub Usage

[📺 GitHub Pull Request Tutorial](https://www.youtube.com/watch?v=jRLGobWwA3Y)

[📘 Feature Branch Workflow Reference](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)

[📺 Azure DevOps - Github connection](https://dev.to/pwd9000/integrating-azure-devops-with-github-hybrid-model-3pkg)

- **Repository Management**:
  - Repos are structured per project/component as needed
- **Branch Strategy**:
  - Two main branches: `development` (default for development), `main` (production-ready)
  - Feature and Bug branches: `feature/<ticket-id>-short-description` or `bug/<ticket-id>-short-description` — this is just a naming convention. The word `feature/` is not a folder; it's part of the branch name to organize and identify branches logically (e.g., `feature/123-login-form`).
- **Code Review Rules**:
  - PRs will be reviewed by another team member before merging
  - User stories of reviewed PRs will be merged and closed by the reviewer
- **Commit Linking Requirement**:
  - Every commit must be linked to an Azure DevOps user story or bug by including the work item ID in the commit message using the AB#{id} syntax. [Click here for more infomation about linking](https://learn.microsoft.com/en-us/azure/devops/boards/github/link-to-from-github?view=azure-devops#use-ab-to-link-from-github-to-azure-boards-work-items)
  - Example: AB#28 this commit is a test

    ![Azure User Story Github linking](../profile/user_story_github_linking.png?raw=true)

- **CI/CD Integration**:
  - Currently not in use — CI/CD will be set up at a later stage

---

### 4. Azure DevOps Usage

- **Work Item Hierarchy**:

| Hierarchy Level  | Description                                                                                | Approximate Time Required | Example                                               |
| ---------------- | ------------------------------------------------------------------------------------------ | ------------------------- | ----------------------------------------------------- |
| Epic             | High-level product goals that group multiple features                                      | Weeks to months           | chatbot MVP                                             |
| Feature          | A collection of related user stories that fulfill a product objective                      | Several days to a week    | Make chatbot answer efficiently                         |
| User Story / Bug | User stories are for new features or improvements. Bugs are defects that need to be fixed. | A few hours to 3 days     | Fine-tune chat completion model / Quang: File exports |
| Task             | Subtasks linked to user stories for detailed implementation                                | About 1 hour              | Add the fine tuned model in the DB scheme excel file  |

- **Project Management**:
  - Everyone is responsible for keeping the board up-to-date. It is not the responsibility of the team lead to clean it up.
  - Use the [**Board**](XXX) view to track sprint-specific tasks
  - Use the [**Backlog**](XXX) view to manage overall structure (Epics > Features > User Stories/Bugs)
- **Board Columns**:
  - **New**: Newly added work items
  - **Active**: Currently in progress
  - **Blocked / Waiting for**: Progress is stalled due to dependencies on others
  - **Review**: Work completed and ready for review by Maris or Lucas
  - **Closed**: Reviewed and accepted
- **Work Item Types**:
  - **User Stories**: For new features or improvements
  - **Bugs**: For defects that need fixing

---

### 5. Communication & Meetings

- **Sprint Length**: TBD
- **weekly checkups**: 13:30 on Tuesdays

---

### 6. Good Practices

- Use **Python version 3.11.7** for all development
- Use **uv** to create and manage Python environments
  - Documentation: [uv environments](https://docs.astral.sh/uv/pip/environments/#discovery-of-python-environments)


