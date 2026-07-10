# Security Policy

## Reporting a Security Issue

The Agent Asset Registry is a catalog of AI agent types, not a software runtime. However, security issues can arise in several ways:

1. **Inaccurate or misleading agent type entries** — An entry that understates risk, misrepresents capabilities, or omits known dangerous behaviors
2. **Vulnerabilities in the registry tools** — Validation, search, or reporting scripts that could be exploited
3. **Malicious contributions** — Entries containing harmful content, misinformation, or attempts to subvert the schema
4. **Disclosure of unreported agent vulnerabilities** — Information about agent types with security implications that may not be widely known

### How to Report

**Do not open a public GitHub issue for security-sensitive reports.**

Instead, send a detailed report to **security@nousresearch.com**. You will receive an acknowledgment within 48 hours.

### What to Include

To help us triage and respond effectively, please include:

- **Type of issue** (inaccurate entry, tool vulnerability, malicious content, disclosure)
- **Agent type ID or file path** (if applicable)
- **Description** — What the issue is and why it matters
- **Impact** — Who could be affected and how
- **Suggested remediation** — How you think the issue should be addressed (optional)
- **Supporting evidence** — Links, screenshots, references, or research

### What to Expect

1. **Acknowledgment** within 48 hours
2. **Triage** within 5 business days — we assess severity and determine next steps
3. **Resolution** — We work with the reporter to address the issue, which may include:
   - Updating or removing registry entries
   - Patching tools
   - Reverting malicious contributions
   - Coordinated disclosure with affected parties

### Responsible Disclosure

We ask that you give us reasonable time to address the issue before public disclosure. We will coordinate disclosure timing with you.

## Security Considerations for Registry Consumers

### Risk Profiles

Each agent type entry includes a `risk_profile` field (low / medium / high / critical). This reflects the **potential** risk of the agent type, not any specific deployment. Always perform your own risk assessment before allowing any agent type into your environment.

### Detection Signatures

The `detection_signatures` field provides indicators that can help identify an agent type in runtime environments. These are not exhaustive and may not cover all variants. Use them as a starting point for your own detection rules.

### Verification

We encourage registry consumers to independently verify agent type information, especially before making security decisions. The registry is a community resource and cannot guarantee the accuracy of every entry.

## Supported Versions

| Version | Status |
|---------|--------|
| 1.x     | ✅ Active — receiving updates |

## Security Updates

Security-related updates will be documented in GitHub release notes. Subscribe to releases to stay informed.

---

*Security of the AI agent ecosystem is a shared responsibility. Thank you for helping keep this registry trustworthy.*
