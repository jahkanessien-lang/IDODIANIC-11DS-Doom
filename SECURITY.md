# Security Model

## Threat assumptions

11DS assumes attackers may obtain credentials, compromise endpoints, exploit software defects, abuse cloud control planes, manipulate dependencies, exploit human error, or attempt to misuse AI-enabled automation.

## Security properties

- Least privilege
- Deny by default
- Separation of duties
- Strong authentication
- Segmentation
- Cryptographic integrity
- Immutable or tamper-evident evidence where appropriate
- Recovery from trusted state
- Independent assurance

## Public repository rules

Never commit:
- secrets or credentials
- private certificates/keys
- production configuration
- customer data
- internal network maps
- recovery procedures that would materially weaken a real deployment

Use secret scanners and dependency/security checks in CI before publication.
