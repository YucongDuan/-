# Security Policy

## Reporting

Do not submit real patient data, passwords, certificates, access tokens or live hospital endpoint details in a public issue. Report security concerns through an approved private channel selected by the deploying organization.

## Production requirements

- Disable all demo credentials and tokens.
- Terminate TLS at a hospital-approved gateway and use mTLS where required.
- Trust identity headers only from configured proxy CIDRs.
- Store secrets in a KMS/HSM or approved secret manager, never in Git.
- Keep PHI payload logging disabled by default.
- Apply least privilege, separation of duties and periodic access review.
- Perform dependency/image, configuration, source and penetration testing in the deployment environment.
- Connect audit and security events to the hospital SIEM.
- Exercise backup, restoration, key rotation and incident response before go-live.

## Clinical safety

The integration layer must not autonomously diagnose, prescribe, determine dosage, select acupuncture points, submit medical orders or replace emergency workflows. External content enters a reversible staging area and requires authorized human review.
