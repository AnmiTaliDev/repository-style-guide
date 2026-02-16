# Legal & Security Files

Files that address legal, security, and compliance concerns. Increasingly important for professional projects.

## SECURITY

Defines how to report security vulnerabilities responsibly.

### Required Contents
- How to report vulnerabilities (email address, security form URL, encrypted communication methods)
- Expected response time for security reports
- Disclosure policy and timeline
- List of supported versions
- Security update policy
- Hall of fame or acknowledgment policy for reporters
- What qualifies as a security issue

### Platform Integration
GitHub recognizes `SECURITY.md` and adds a "Security" tab to repositories, making it easily discoverable.

### Naming Variants
- `SECURITY.md`
- `SECURITY`
- `VULNERABILITIES.md`
- `SECURITY_POLICY.md`
- `POLICY.md`

### Critical Requirements
- Private reporting mechanism
- Clear statement to NOT open public issues for vulnerabilities
- Designated security contact
- Expected timeline for response and fixes

## PRIVACY

Privacy policy for projects that collect user data.

### When Required
- Applications that collect user data
- Services with user accounts
- Projects with analytics or telemetry
- Required by GDPR, CCPA, and other regulations
- Any data processing activities

### Required Contents
- Types of data collected
- Purpose of data collection
- How data is used and stored
- Data retention policies
- Third-party services involved
- User rights (access, deletion, portability)
- Contact information for privacy inquiries
- Data security measures
- Cookie usage (if applicable)
- Changes to privacy policy procedures

### Naming Variants
- `PRIVACY.md`
- `PRIVACY`
- `PRIVACY_POLICY.md`
- `DATA_USAGE.md`
- `GDPR.md`

## TRADEMARK

Guidelines for using project name, logo, and branding.

### Required Contents
- Allowed uses of name and logo
- Restrictions and prohibited uses
- Attribution requirements
- Logo file locations and specifications
- Modification permissions
- Commercial use policies
- Required clearances or approvals

### When to Include
- Projects with recognizable brands
- Projects preventing name confusion
- Organizations with trademark registrations
- Projects with official logos or visual identity

### Naming Variants
- `TRADEMARK.md`
- `TRADEMARK`
- `BRAND_GUIDELINES.md`
- `LOGO.md`
- `BRANDING.md`

## NOTICE

Legal notices and attributions, common in Apache 2.0 projects.

### Required Contents
- Third-party licenses and attributions
- Patent notices
- Legal disclaimers
- Copyright notices
- Required acknowledgments from dependencies

### When Required
- Apache 2.0 license requires NOTICE file
- When using dependencies with attribution requirements
- For patent grant notifications

### Naming Variants
- `NOTICE`
- `NOTICE.md`
- `LEGAL.md`
- `LEGAL`
- `DISCLAIMER.md`
- `DISCLAIMER`

## DCO (Developer Certificate of Origin)

Certifies that contributors have the right to submit their code.

### What It Is
A lightweight alternative to CLAs where contributors sign-off on commits using git's built-in signing mechanism.

### How It Works
Contributors add sign-off to commits certifying they have rights to submit the contribution under the project's license.

### When to Use
- Projects wanting legal clarity without heavy CLAs
- Open source projects (Linux kernel uses this)
- When contributor agreement is needed but CLA is too burdensome
- Should NOT be used simultaneously with CLA

### Naming Variants
- `DCO`
- `DCO.md`
- `DEVELOPER_CERTIFICATE.md`

### Required Contents
- Full text of Developer Certificate of Origin
- Instructions for signing commits
- Explanation of what DCO means
- Enforcement policy

## CLA (Contributor License Agreement)

Legal agreement for contributors. **Use with caution.**

### Warning
CLAs are controversial and can discourage contributions. Consider DCO as a lightweight alternative for most projects.

### When Companies Use CLAs
- Managing intellectual property transfers
- Corporate or enterprise projects
- Projects that may need to relicense
- When copyright assignment is required

### Why CLAs Are Not Recommended for Most Projects
- Creates significant barrier to contribution
- Requires additional infrastructure and management
- Can alienate open source community
- DCO is usually sufficient for legal protection
- Administrative overhead

### Naming Variants
- `CLA.md`
- `CLA`
- `CONTRIBUTOR_LICENSE_AGREEMENT.md`

### If CLA Is Required, Must Include
- Full legal text of agreement
- Signing procedure
- Corporate CLA option
- Justification for CLA requirement
- Electronic signing mechanism
- CLA bot integration information

## Best Practices

1. **SECURITY is essential** - Even small projects can have vulnerabilities
2. **PRIVACY when collecting data** - Required by law in many jurisdictions
3. **Consider DCO over CLA** - Less friction, legally sound
4. **NOTICE for Apache 2.0** - Some licenses require it
5. **TRADEMARK protects brand** - But only for established projects
6. **Keep legal files updated** - Review annually or when regulations change
7. **Get legal advice** - For complex situations, consult a lawyer
8. **Make security reporting easy** - Clear, accessible process
9. **Be transparent** - Legal documents should be easily findable
10. **Don't overburden contributors** - Balance legal protection with accessibility
