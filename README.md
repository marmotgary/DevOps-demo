# DevOps-demo
This repository servers as a demo for setting up a DevOps Pipeline. 

# Tooling
Listing of tools we have found useful. Lots of alternatives for each and every one of them exists out there!


## Developer
Tooling used on Developers local environment

### Pre-commit Hooks

#### Talisman
https://github.com/thoughtworks/talisman

Talisman is a tool that installs a hook to your repository to ensure that potential secrets or sensitive information do not leave the developer's workstation. It validates the outgoing changeset for things that look suspicious - such as potential SSH keys, authorization tokens, private keys etc.

We have Talisman installed on our local workstations as a pre-commit git hook template.

### Linters
Set up a linter into your IDE, depends on the language you are developing on. Git hooks for example could also be used to enforce project coding standards.

### IDE Plugins
There are lots of plugins for every IDE out there, that boosts greatly boosts productivity and minimizes errors.  For example some I've installed on my VSCode: Docker, ESLint, GitHub Actions, GitLens, Remote - WSL 


## Infrastructure as Code

### Docker
https://www.docker.com/

### Kubernetes
https://kubernetes.io/

## Security

### Njsscan
https://github.com/ajinabraham/njsscan#github-action

Njsscan is an open source Statis Application Security Testing (SAST) tool that aims to find insecure code patterns in node.js applications, and is currently integrated to our CI/CD pipeline workflow.

It utilizes libsast pattern matcher and the syntax-aware semantic code pattern search tool semgrep, and is set to run on every push to our development branch and scan the entire project.

### OWASP ZAP Full Scan
https://github.com/marketplace/actions/owasp-zap-full-scan

OWASP ZAP (Zed Attack Proxy) Full Scan is an open source Dynamic Application Security Testing (DAST) tool that is designed to perform automated security scans against applications and their environment.

The ZAP Full Scan runs the ZAP spider and optionally also an ajax spider scan against the specified target site. The tool then reports it's findigs and automatically creates GitHub issues to the corresponding project in case it finds something alarming.

## Monitoring

# Resources
## DevOps
* https://roadmap.sh/devops
## DevSecOps
* https://notsosecure.com/achieving-devsecops-with-open-source-tools/
* https://medium.com/fraktal/practical-framework-for-devsecops-dd7fd9e63866
