# Security Policy

## Supported Versions

We actively maintain and provide security updates for the latest versions of all Minisource projects.

| Version | Supported          |
| ------- | ------------------ |
| latest (main branch) | :white_check_mark: |
| Previous releases | :x: |

## Reporting a Vulnerability

**If you discover a security vulnerability, please DO NOT open a public issue.**

### How to Report

Email us directly at: **security@minisource.ir**

Please include:
- Description of the vulnerability
- Steps to reproduce
- Affected repository/service
- Potential impact
- Suggested fix (if any)

### What to Expect

1. **Acknowledgment**: We will acknowledge your email within **48 hours**
2. **Assessment**: We will assess the vulnerability and provide a detailed response within **5 business days**
3. **Fix & Disclosure**: Once fixed, we will:
   - Release a security patch
   - Credit you in the release notes (if desired)
   - Publish a security advisory

### Responsible Disclosure

We ask that you:
- Give us reasonable time to fix the issue before public disclosure
- Do not exploit the vulnerability beyond what is necessary to demonstrate it
- Keep vulnerability details confidential until we publish a fix

## Security Best Practices

For all Minisource services:
- Keep dependencies up to date (Dependabot enabled)
- Use environment variables for secrets
- Enable 2FA on GitHub
- Review security advisories regularly
- Follow least privilege principles

## Security Features

All Minisource projects include:
- Automated dependency scanning (Dependabot)
- Secret scanning and push protection
- Regular security audits
- Secure coding guidelines
- Input validation and sanitization

## Scope

This security policy applies to all repositories under the **minisource** GitHub organization:
- All core services (auth, gateway, storage, etc.)
- All SDKs (go-sdk, csharp-sdk)
- All shared libraries (go-common, csharp-common)
- Infrastructure and templates

## Bug Bounty

We currently do not have a bug bounty program, but we greatly appreciate responsible disclosure and will acknowledge contributors in our release notes.

## Contact

- **Security Email**: security@minisource.ir
- **General Contact**: info@minisource.ir

---

Thank you for helping keep Minisource and our users safe!
