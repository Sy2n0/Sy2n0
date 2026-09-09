![CVEs](https://img.shields.io/badge/CVEs-7-red?style=for-the-badge)
![Hall-of-Fame](https://img.shields.io/badge/Hall_of_Fame-3-green?style=for-the-badge)

## About Me

- Security Researcher / CTF Player @[W4llz](https://w4llz.me/)

***

## Awards

| Year | Name | Award |
|------|------|-------|
| 2026 | Jiyong | MSRC - Special Mentions |
| 2026 | Jiyong | NASA VDP (Vulnerability Disclosure Program) - Hall of Fame |
| 2026 | W4llz | SekaiCTF 2026 2nd |
| 2025 | Jiyong | Google Cloud VRP (Vulnerability Reward Program) - Honorable Mention |

***

## CVEs

<details>
<summary><b>CVE-2026-81379 — VS Code Marketplace Policy Bypass via URL Canonicalization</b></summary>

**Target**
- microsoft/vscode

**Summary**

- VS Code incorrectly derives the enterprise-policy identity of a GitHub Agent Plugin marketplace before fully canonicalizing its repository URL.
- An attacker can craft a repository path containing traversal components (`../`) so that VS Code validates it as an allowlisted marketplace while Git resolves the same URL to an attacker-controlled repository.
- This discrepancy allows an unauthorized marketplace to bypass `chat.plugins.strictMarketplaces`, install an attacker-controlled Agent Plugin, and execute its configured hooks during normal chat interactions.
- The vulnerability is a security feature bypass that can lead to remote code execution (CWE-180: Validate Before Canonicalize).


**References**
- CVE: https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-81379
</details>


<details>
<summary><b>CVE-2026-58043 — Permission Model Filesystem Allowlist Bypass in Node.js</b></summary>

**Target**
- nodejs/node

**Summary**
- Improper enforcement in the Node.js Permission Model that can over-grant filesystem access across radix-tree prefix boundaries.
- Under `--permission`, an attacker granted access to one path could abuse boundary handling to read from or write to paths outside the intended filesystem allowlist.
- Affected: Node.js main, 22.x, 24.x, 26.x.

**References**
- CVE: https://hackerone.com/hacktivity/cve_discovery?id=CVE-2026-58043
</details>

<details>
<summary><b>CVE-2026-15921 — LTS Alias Path Traversal in nvm</b></summary>

**Target**
- nvm-sh/nvm

**Summary**
- Path traversal vulnerability caused by insufficient validation of mirror-supplied LTS codenames.
- A malicious or compromised Node.js mirror could write outside `$NVM_DIR/alias/lts` and overwrite shell startup files such as `~/.bashrc`, `~/.zshrc`, or `~/.profile`, potentially leading to command execution when the shell starts.

**References**
- Advisory: https://github.com/nvm-sh/nvm/security/advisories/GHSA-4ghp-wxpw-rhpg
- CVE: https://www.cve.org/CVERecord?id=CVE-2026-15921

</details>

<details>
<summary><b>CVE-2026-48718 — Firebird</b></summary>

**Status**
- Coordinated disclosure (technical details will be published after the embargo).

</details>

<details>
<summary><b>CVE-2026-1665 — Command Injection in nvm</b></summary>

**Target**
- nvm-sh/nvm

**Summary**
- Command injection caused by insufficient validation of environment variables during `wget` invocation.

**References**
- Advisory: https://github.com/nvm-sh/nvm/security/advisories/GHSA-4fc5-r4vr-8rp7
- CVE: https://www.cve.org/CVERecord?id=CVE-2026-1665

</details>

<details>
<summary><b>CVE-2025-69262 — Command Injection in pnpm</b></summary>

**Target**
- pnpm/pnpm

**Summary**
- Command injection through environment variable substitution, potentially leading to arbitrary code execution in CI/CD and build environments.

**References**
- Advisory: https://github.com/advisories/GHSA-2phv-j68v-wwqx

</details>

<details>
<summary><b>CVE-2025-14550 — Denial of Service in Django</b></summary>

**Target**
- django/django

**Summary**
- Super-linear processing of repeated HTTP headers in the ASGI request path, enabling a potential denial-of-service attack.

**References**
- Advisory: https://github.com/advisories/GHSA-33mw-q7rj-mjwj

</details>

***

## Contact

- **Name**: Jiyong Yang (양지용)
- **Contact**: contact@sy2n0.me
