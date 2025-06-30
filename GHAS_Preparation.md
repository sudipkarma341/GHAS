
Q1: Which Dependabot comment command will get a pull request successfully completed?

```
@dependabot merge
```
This command tells Dependabot to merge the pull request if all requirements are met.

Q2: Is GitHub dependency graph available for free to all repositories?

Yes, it's available for free for all repositories.

Q3: Where can you see when the last CodeQL analysis was run when using the default code scanning setup?

- In the code scanning tool status page

Q4: Can you use CodeQL analysis with third party CI systems?

Yes, CodeQL analysis can be run with third party CI systems by using the CodeQL CLI to perform analysis and upload results to GitHub.

Q5: Which of these statements are true regarding running CodeQL analysis on codebases with multiple programming languages? (Choose two.)

- CodeQL creates separate databases for each programming language.
- CodeQL uses a different extractor for each programming language.

Q6: What are the three different sets of secret scanning patterns that GitHub maintains? (Select three.)

- User alert patterns
- Partner patterns
- Push protection patterns

Q7: What is the behavior when a new secret pattern is added or updated in the GitHub secret scanning partner program?

- GitHub will run a scan of all historical code content in public repositories with secret scanning enabled.

Q8: Which parts of the repository are scanned by secret scanning? (Choose two.)

- Entire git history on all branches in the repository
- Titles, descriptions and comments in open and closed historical issues

Q9: What is QL?

- QL is a query language that underlies CodeQL.

Q10: What does CVE stand for?

- Common Vulnerabilities and Exposures

Q11: Jobs that run on macOS runners that GitHub hosts consume minutes at __ rate as Linux runners consume

- 10x the rate

Q12: The tool that checks if a pull request introduces any dependencies with security vulnerabilities is called:

- Dependency Review

Q13: What happens when a second SARIF results file is uploaded to GitHub for a single commit?

- It replaces the original set of data.

Q14: Dependabot Alerts are enabled by default on:

- Dependabot Alerts are not enabled by default on any repositories. 

Q15: CodeQL scanning supports:

- Both compiled and interpreted languages.

Q16: Which of these is a valid dependabot.yml configuration file?


- The following is a valid `dependabot.yml` configuration file:

    ```yaml
    version: 2
    updates:
        - package-ecosystem: "npm"
            directory: "/"
            schedule:
                interval: "daily"
    ```



Q17: When using GitHub Actions as your CI system and a third party tool to run code scanning, how can you upload the SARIF results to GitHub?

- By using the `github/codeql-action/upload-sarif` GitHub Action.


Q18: How can you exclude certain directories or files from secret scanning?
- By creating a secret_scanning.yml file and including paths that should not be scanned

Q19: Which of these best describes secret scanning?

- Secret scanning scans your repository for secrets such as private keys or tokens.

Q20: If you don't want to use GitHub Actions, you can run code scanning in an external CI system, then upload the results to GitHub.

- True

Q21: In what format can you export the GitHub Dependency graph of your repository?

- You can export the GitHub Dependency graph in the SPDX format.

Q22: You have accidentally committed your GitHub personal access token to a public repository. What actions should you take to prevent your account from being compromised?

- Consider the token compromised and delete it immediately

Q23: Which of these statements best defines a vulnerable dependency?

- A vulnerable dependency is a dependency that a project relies on, which contains security flaws that could potentially be exploited, compromising the project's security.

Q24: How can you enable GitHub Advanced Security features on GitHub Enterprise Server? (Choose two.)

- In the Security tab of the Site admin management console
- By connecting directly to the GitHub Enterprise Server instance through SSH and using the administrative shell `ghe-config` commands.

Q25: What details can you find on a code scanning alert page? (Choose three.)

- Branches affected by the vulnerability
- Severity of the vulnerability
- Highlighted vulnerable code


Q26: Which GitHub Action can be used to upload a third-party SARIF file?

- The `github/codeql-action/upload-sarif` GitHub Action can be used to upload a third-party SARIF file.

Q27: Which of these is true about the GitHub secret scanning partner program? (Choose three.)

- When GitHub identifies a secret from a partnered service provider, it notifies the service provider about the leaked secret.
- It is a program where service providers can provide GitHub with the regex patterns of secrets that they issue so GitHub secret scanning can recognize them.
- The partner can take actions upon receiving notification from GitHub about a leaked secret, such as revoking the secret and informing the owner of the compromised secret.

Q28: What information do Dependabot alerts provide?

- Dependabot alerts tell you that your repository uses a package that is insecure.

- Query packs
- Library packs
- Model packs

Q30: Which tool can be used in a third-party CI system to upload code analysis results to GitHub?

- CodeQL CLI

Q31: Which of these statements about Dependabot Alerts are true? (Choose three.)

- When GitHub identifies a vulnerable dependency, they generate a Dependabot alert and display it on the Security tab for the repository
- To enable Dependabot Alerts you first need to have Dependency Graph enabled on your repository
- They partially rely on the GitHub Advisory Database

Q32: What are CodeQL queries used for?

- CodeQL queries can be run against a CodeQL database to identify patterns that may indicate coding errors or security vulnerabilities.

Q33: What's the purpose of the Secret scanning partner program?

- Service Providers can partner with GitHub so that the format of their secrets can be recognized by GitHub secret scanning.

Q34: As a repository maintainer where should you put instructions on how to report a security vulnerability in your codebase?

- In the `SECURITY.md` file

Q35: Which key should be used in a secret_scanning.yml file to exclude directories from secret scanning alerts in GitHub?

- `paths-ignore`

Q36: What is CodeQL?

- CodeQL is a code analysis engine developed by GitHub that allows you to query code as though it were data, enabling the identification of security vulnerabilities and coding errors.


Q37: How can you configure your GitHub repository to run CodeQL analysis on a schedule? (Choose two.)

- By creating a GitHub Actions workflow with a `schedule` trigger that uses actions from the `github/codeql-action` repository.
- By using the default CodeQL analysis setup, which automatically configures scheduled analysis.

Q38: What is CodeQL?

- CodeQL is a code analysis tool.

Q39: How does GitHub Dependency graph know what dependencies your project is using? (Choose two.)

- Dependencies can be manually added using the Dependency submission API.
- GitHub derives dependencies automatically from manifests and lock files committed to the repository.

Q40: Which of these is NOT a valid approach one can take to reduce the time it takes for CodeQL analysis workflow to complete?

- Run the analysis on every push event

Q41: Which of these is true about code scanning? (Choose two.)

- Code scanning helps finding insecure code patterns which can be missed by manual code review.
- Code scanning can be integrated into the CI pipeline to find security issues early in the development process.

Q42: An organization has recently started using CodeQL analysis for all pull requests on their repositories as well as running the analysis on an hourly schedule. Since then they are experiencing larger than usual GitHub Actions bills. What is the most likely cause of this?

- Code scanning uses GitHub Actions and the organization is being billed for the additional usage.


Q43: Which of the following languages is NOT supported by CodeQL for code scanning?

- PHP

Q44: How does CodeQL analyze code in GitHub?

- It generates a CodeQL database and runs queries to identify problems, displaying results as code scanning alerts.


Q45: How can you set a default security policy for all repositories in my-org GitHub Organization?

- By creating a `SECURITY.md` file in the `my-org/.github` repository. 

Q46: Fill in the blank: GitHub __________ is a feature that you can use to analyze code in a GitHub repository to find security vulnerabilities and coding errors.

- Code Scanning

Q47: What is the purpose of the external-repository-token parameter in github/codeql-action/init GitHub Action?

- It allows the action to access a private GitHub repository that contains configuration files, queries or packs that are required for the analysis

Q48: When GitHub runs a scan of all historical code in enterprise repositories what is the notification behavior? (Select two.)

- GitHub notifies the enterprise owners and security managers, even if no secrets are found.
- GitHub notifies Repository administrators, security managers, and users with custom roles with read/write access whenever a secret is detected in a repository.

Q49: What is a CodeQL query suite?

- A CodeQL query suite is a collection of CodeQL queries 

Q50: You need GitHub Actions enabled for

- Dependency Review

Q51: What is required for a CI server to upload SARIF results to GitHub?

- A GitHub App or personal access token with `security_events: write` permission is required for a CI server to upload SARIF results to GitHub.

Q52: What does it mean to dismiss a code scanning alert?

- Closing an alert that you don't think needs to be fixed

Q53: To enable Dependabot Alerts on all repositories in an organization you should:

- Go to the organization's Code security and analysis settings and enable Dependabot Alerts for all repositories at once.

Q54: What does CWE stand for?

- Common Weakness Enumeration

Q55: What do Dependabot alerts indicate in GitHub?

- The presence of a vulnerable dependency or malware in your repository


Q56: What is the maximum number of custom patterns that can be defined for secret scanning on GitHub?

- 500 for organizations and enterprises, and 100 for repositories.


Q57: When using CodeQL analysis in your GitHub Actions workflow, how often is the scan triggered?

- Code scanning can be triggered for many different events that happen in the repository.

Q58: Multiple public repositories that you are contributing to do not have secret scanning push protection option enabled. What can you do to protect yourself from accidentally pushing secrets to these repositories?

- Enable Push protection for yourself, in your personal GitHub account settings

Q59: What does CVSS stand for?

- Common Vulnerability Scoring System

Q60: How can you automate dismissing low severity Dependabot alerts?

- By using Dependabot's auto-triage rules.


Q61: How can users exclude specific directories from secret scanning alerts on GitHub?

- By configuring a `secret_scanning.yml` file under the `.github` directory in the repository and specifying the directories to exclude using the `paths-ignore` key.


Q62: How can you prevent commits containing cloud provider credentials from being pushed to GitHub?

- Enable a secret scanning push protection rule for your repository or organization.


Q63: Is secret scanning available for both public and private repositories on GitHub?

- Yes, but for private repositories, it requires a license for GitHub Advanced Security.

Q64: Does GitHub use the same set of secret scanning patterns for both user alerts and push protection alerts?

No, GitHub uses different sets of secret scanning patterns for user alerts and push protection alerts.

Q65: What are Dependabot auto-triage rules?

- It's a feature that allows Dependabot to automatically dismiss Dependabot alerts that match certain criteria.

Q66: Can your repository use Dependency Graph without using Dependabot Alerts?

Yes, you can use the Dependency Graph feature in your repository without enabling Dependabot Alerts. Dependency Graph works independently to show your project's dependencies.

Q67: As part of your Jenkins CI pipeline you've successfully created and then analyzed a CodeQL database, therefore producing a SARIF file. How can you upload the SARIF file to GitHub? (Choose two.)

- Using the codeql github upload-results command from CodeQL CLI
- Using the GitHub REST API `POST /repos/{owner}/{repo}/code-scanning/sarifs` endpoint


Q68: What is a CodeQL query pack?

- It's a set of pre-compiled queries with all transitive dependencies such as libraries and models.

Q69: Which of these statements isn't true about secret scanning on GitHub?

- Secret scanning is a tool for secure secret storage and management.

Q70: What is the purpose of code scanning in GitHub?

- To identify vulnerabilities and errors in code

Q71: Who can enable Dependabot alerts on a repository?

- Repository owners and people with admin access can enable Dependabot alerts on a repository.

Q72: Which API endpoint can be used to retrieve a list of all Dependabot alerts for an enterprise?

- `GET /enterprises/{enterprise}/dependabot/alerts`


Q73: What is a GitHub security policy?

- It's a document that instructs users on how to responsibly report security vulnerabilities in a project. It's typically defined in a SECURITY.md file in a repository.

Q74: To enable Dependabot security updates on all repositories in an organization you should:

- Go to the organization's Code security and analysis settings and enable Dependabot Security Updates for all repositories at once.

Q75: What does shifting left mean in the context of Security?

- Adopting security practices early in the development cycle

Q76: What are Repository Security Advisories?

- A private space where repository maintainers can discuss vulnerabilities and security issues within the codebase.

Q77: Public repositories owned by personal users as well as public repositories owned by organizations can use secret scanning for free.

- True. Secret scanning is available for free on all public repositories, regardless of whether they are owned by individuals or organizations.

Q78: Which API endpoint can be used to retrieve a list of all code scanning alerts for a repository?

- `GET /repos/{owner}/{repo}/code-scanning/alerts`


Q79: What is the purpose of defining a SARIF category?

- Use the category to distinguish between multiple analyses for the same tool or commit, but performed on different languages or different parts of the code.

Q80: Which of these statements regarding viewing the results of a CodeQL analysis are true? (Choose two.)

- You need write permission to view a summary of all the alerts for a repository in the Security tab.
- Anyone with read permission for a repository can see code scanning annotations on pull requests.

Q81: How can you customize your advanced CodeQL scanning setup with additional CodeQL query suites? (Choose two.)

- By defining the customizations in the CodeQL analysis GitHub Actions workflow as input parameters to the github/codeql-action/init action
- By using a custom configuration file and defining additional queries there.


Q82: What is the GitHub dependency graph?

- It is a representation of a repository's dependencies and dependents.

Q83: You have included some fake secrets in your test code and they have been picked up by GitHub's secret scanning. What can you do to tell GitHub that these are fake secrets used in tests and can be ignored by secret scanning? (Choose two.)

- By creating a `secret_scanning.yml` file within the `.github` directory and specifying the paths where fake secrets are located, so scans will omit them.
- Close the Secret Scanning Alert with the "Used in tests" close reason.

Q84: What are Dependabot security updates?
- It's a Dependabot feature that automatically creates pull requests to update vulnerable dependencies in your repository.

Q85: When using a third party CI system to run code scanning, what GitHub tool do you need to analyze the codebase?

- You don't specifically need a GitHub tool, any static analysis tool that can produce results in SARIF format will work.

Q86: What are the differences when running CodeQL database creation for compiled and interpreted languages? (Choose two.)

- For compiled languages, extraction works by monitoring the build process and collecting information each time the compiler is invoked to process a source file.
- For interpreted languages, the extractor runs directly on the source code.

Q87: How can you enable GitHub Advanced Security features for all repositories in an organization in GitHub Enterprise Cloud?

- In Code security and analysis section of the organization settings

Q88: What CodeQL CLI command is used to create a CodeQL database?

- The command is:
  
  ```
  codeql database create
  ```

Q89: Which API endpoint can be used to retrieve a list of all secret scanning alerts for an organization?

- `GET /orgs/{org}/secret-scanning/alerts`

Q90: How can you use a custom CodeQL configuration file in a GitHub Actions workflow?

- By explicitly providing the configuration file path in the config-file input parameter of the github/codeql-action/init action

Q91: Where can you specify the CodeQL queries to run in a GitHub Actions workflow? (Choose two.)

- In the `queries` input parameter of the `github/codeql-action/init` action
- In a CodeQL configuration YAML file


Q92: Which top-level keys are required in the dependabot.yml file?

- `version` and `updates`

Q93: When will the GitHub Dependency graph for your repository be updated? (Choose two.)


- When you push a commit to the repository's default branch, only if that changes or adds a supported manifest/lockfile.
- When anyone pushes a change to the repository of one of your dependencies.

Q94: How can CodeQL be used in an external CI system together with GitHub repositories?

- Run CodeQL CLI in the external CI system to scan code and upload the results to the GitHub repository

Q95: Which feature is a pre-requisite for using Dependabot Alerts on a repository?

- Dependency graph

Q96: What is extraction in the context of CodeQL code analysis?

- Extraction is the process of creating a relational representation of each source file in the codebase.

Q97: What is the main purpose of using the CodeQL CLI?

- To generate a database representation of a codebase, a CodeQL database

Q98: What's the lowest access level needed to see Dependabot alerts in a repository within an organization?

- Write

Q99: What does the default CodeQL analysis setup in GitHub do?

- Automatically chooses languages to analyze, query suite to run, and events that trigger scans

Q100: When a CodeQL analysis GitHub Actions workflow detects a new vulnerability on a pull request, where can you find the information about that vulnerability?

- Directly in the pull request in the form of a PR comment and a check failure

Q101: Which GitHub Advanced Security feature allows you to find, triage, and prioritize fixes for new and existing problems in your code?

- Code scanning

Q102: Who will be notified when a NEW secret is pushed and detected in a repository? (Choose five.)

- Repository Administrators
- Security Managers
- Commit authors
- Users with custom roles with read/write access
- Organization owners and enterprise owners, but only if they are administrators of repositories where secrets were leaked

Q103: When viewing a code scanning alert what is the Show paths option used for?

- It will display the path through the code that leads to the issue causing the alert.

Q104: Which of the following statements about enabling CodeQL scanning default setup are true? (Choose three.)

- GitHub Actions need to be enabled as a prerequisite
- You can enable default setup on any repository, regardless of the contents of the repository
- You can enable default setup for all eligible repositories in an organization at once in the organization settings

Q105: Which of these is not a GitHub supported channel for receiving Dependabot alerts?

- SMS/CALL

Q106: What are the primary benefits of the Security Overview feature in GitHub?

- Centralized view of security alerts and policy management in an organization

Q107: What are the steps of CodeQL analysis workflow?

- Creating a CodeQL database -> Running CodeQL queries -> Interpreting the results

Q108: Which of the following is a curated list of security vulnerabilities found in open source projects?

- GitHub Advisory Database

Q109: What is the effect of adding the paths-ignore keyword to your code scanning GitHub Actions workflow?

.github/workflows/codeql-analysis.yml

on:
  pull_request:
    branches: [main]
    paths-ignore:
      - '**/*.md'
      - '**/*.txt'

- Avoiding unnecessary scans when files that are not relevant to the analysis are changed.


Q110: When running CodeQL analysis in GitHub Actions, what Actions should you use? (Choose three.)

- `github/codeql-action/init`
- `github/codeql-action/autobuild only for compiled programming languages`
- `github/codeql-action/analyze`

Q111: What is the purpose of the codeql database analyze command in CodeQL CLI?

- Analyzing a CodeQL database, producing results usually in the form of a SARIF file.

Q112: What is the simplest method to execute CodeQL analysis concurrently for each language in a multi-language repository using GitHub Actions?

- By creating a languages matrix for the job and then reference it in the github/codeql-action/init action's languages input parameter

Q113: How can you enable code scanning for a repository?

- Go to the security tab of the repository settings and enable code scanning with default or advanced setup.

Q114: Which of these GitHub security features are available for FREE for both public and private personal repositories? (Choose four.)

- Security Policy
- Security advisories
- Dependabot version updates
- Dependabot alerts and security updates

Q115: Which tool helps you keep the repository dependencies up to date?

- Dependabot

Q116: Your company has internal secrets that should not be pushed to GitHub repositories. The pattern of these secrets is not known by GitHub and therefore is not detected by secret scanning. What can companies do to protect their developers from accidentally pushing these secrets to repositories in their GitHub Organization?

- Define regex patterns for these secrets and enable custom patterns for secret scanning for the organization.


