# Security Policy

## Supported versions

Security fixes are evaluated for the current public release.

| Version | Supported |
| --- | --- |
| 1.1.4 | Yes |
| Earlier versions | No |

Users should reproduce a suspected issue on Kingdom 1.1.4 before reporting it
when it is safe to do so.

## Reporting a vulnerability

Do not disclose a suspected vulnerability, exploit, sensitive log, or proof of
concept in a public issue.

Report it privately to `pingusama.info@gmail.com`. Use a subject that clearly
identifies the message as a Kingdom security report.

Include, where relevant:

- the Kingdom version;
- the Windows version;
- a concise description of the issue;
- reproducible steps;
- the expected and observed result;
- the potential security impact;
- affected paths or operations;
- minimal screenshots or logs with sensitive data removed.

Do not include personal data, credentials, access tokens, copyrighted game
files, private keys, or unauthorized content or links.

## Security scope

Examples of security-relevant reports include:

- unsafe deletion or path-validation behavior;
- unintended execution of an external file;
- privilege or elevation abuse;
- arbitrary command execution;
- archive traversal, unsafe links, or extraction outside the intended folder;
- insecure handling of configuration or local application data;
- operations that could unexpectedly overwrite or disclose user files.

Normal bugs, compatibility problems, usability feedback, and feature requests
belong in the project's standard issue tracker and should follow
[SUPPORT.md](SUPPORT.md).

## Responsible disclosure

Allow reasonable time for triage and remediation before public disclosure.
Avoid accessing data that is not your own, causing service disruption, or
performing destructive tests. Test only on systems and files that you own or
are authorized to use.

Submitting a report does not grant permission to violate law, access another
person's data, or test systems without authorization.

## Privacy of reports

Kingdom is designed as a local offline utility, but a report may still contain
personal paths, usernames, game-library information, or other sensitive local
details. Redact those details before sending a report and provide only the
minimum information needed to reproduce the issue.

## License boundary

Kingdom's proprietary license does not restrict reverse engineering,
decompilation, disassembly, replacement, relinking, modification, or debugging
to the extent necessary to exercise rights granted by an applicable
third-party license, including the GNU LGPL, or rights that cannot lawfully be
waived. See the canonical Kingdom license for the complete terms.
