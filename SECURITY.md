# Security Policy

## Supported Versions

This Docker template supports the latest stable versions of PHP. Security updates and patches will be applied to the main and actively maintained branches only.

| Version | Supported          |
|---------|--------------------|
| latest  | ✅                 |
| legacy  | ❌ (no longer maintained) |

## Reporting a Vulnerability

If you discover a security vulnerability in this Docker template, **please do not open a public issue**.

Instead, report it privately via email:

**Email:** [soe991398@gmail.com]

Please include:
- A detailed description of the vulnerability.
- Steps to reproduce the issue.
- Any potential impact or exploitability.
- Your contact information for follow-up.

We aim to respond to all valid reports within 5 business days.

## Security Best Practices

To ensure a secure PHP application when using this Docker template:
- Always use official and trusted PHP base images.
- Keep the base image and PHP dependencies up to date.
- Do not store sensitive credentials in the Docker image.
- Use `.env` files or Docker secrets for sensitive configuration.
- Run containers as non-root whenever possible.
- Apply the principle of least privilege in Dockerfile and container runtime settings.

## Dependency Management

This template encourages the use of Composer for PHP dependency management. To minimize vulnerabilities:
- Audit your dependencies using `composer audit`.
- Lock versions using `composer.lock`.
- Use trusted third-party libraries only.

## Updates

Security-related updates will be tagged with a `security` label in GitHub and documented in the CHANGELOG.

## Additional Resources

- [OWASP PHP Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/PHP_Security_Cheat_Sheet.html)
- [Docker Security Best Practices](https://docs.docker.com/engine/security/security/)

