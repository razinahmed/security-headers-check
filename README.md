# Security Headers Check

![Security](https://img.shields.io/badge/Security-Tool-red)
![Bash](https://img.shields.io/badge/Bash-Script-green)
![HTTP](https://img.shields.io/badge/HTTP-Headers-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

An HTTP security headers auditing tool that analyzes web server responses to verify the presence and correctness of security-critical headers.

## Description

Security Headers Check inspects HTTP response headers from web applications and reports on missing or misconfigured security headers. It verifies headers such as Content-Security-Policy, X-Frame-Options, Strict-Transport-Security, and others that protect against common web vulnerabilities like XSS, clickjacking, and MIME sniffing.

## Features

- Scan any URL for security header compliance
- Check for Content-Security-Policy (CSP) headers
- Verify Strict-Transport-Security (HSTS) configuration
- Detect missing X-Frame-Options and X-Content-Type-Options
- Validate X-XSS-Protection and Referrer-Policy headers
- Generate pass/fail reports for each header
- System hardening baseline included
- Makefile-based build and test workflow

## Tech Stack

- **Language:** Bash
- **Tools:** curl, HTTP/HTTPS clients
- **Target OS:** Linux / macOS
- **Build Tool:** GNU Make

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/security-headers-check.git
cd security-headers-check

# Review the scanning script
cat scripts/security_core.sh

# Run the header check against a target URL
bash scripts/security_core.sh
```

## Usage

```bash
# Build and test
make build
make test

# Run the security headers audit
bash scripts/security_core.sh
```

## Project Structure

```
security-headers-check/
  scripts/
    security_core.sh  # Core header auditing script
  Makefile             # Build and test automation
  SECURITY.md          # Security policy
  LICENSE              # MIT License
```

## Contributing

Contributions are welcome. Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
