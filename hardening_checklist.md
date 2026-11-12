
# Security Hardening Checklist – Student Portal

## 1. Introduction

This checklist provides prioritized security improvements for the fictional Student Management Web Application.

The controls are organized according to their security importance.

## 2. Priority 1 – Critical Controls

These controls should be addressed first.

- [ ] Enforce strong password policies.
- [ ] Implement Multi-Factor Authentication (MFA).
- [ ] Store passwords using secure password hashing such as Argon2id.
- [ ] Implement secure session management.
- [ ] Enable HTTPS for all application communication.
- [ ] Prevent unauthorized access to student and administrator accounts.

## 3. Priority 2 – High-Priority Controls

- [ ] Implement Role-Based Access Control (RBAC).
- [ ] Validate all user inputs on the server.
- [ ] Use parameterized database queries.
- [ ] Encrypt sensitive student information.
- [ ] Restrict database access to authorized application services.
- [ ] Protect important application actions with audit logging.
- [ ] Verify permissions before allowing record modifications.

## 4. Priority 3 – Medium-Priority Controls

- [ ] Implement login rate limiting.
- [ ] Monitor unusual login activity.
- [ ] Configure appropriate session expiration.
- [ ] Maintain regular database backups.
- [ ] Configure secure HTTP response headers.
- [ ] Monitor application errors and availability.

## 5. Priority 4 – Continuous Security Practices

- [ ] Regularly update application dependencies.
- [ ] Review user permissions periodically.
- [ ] Perform security reviews after major changes.
- [ ] Test backup restoration periodically.
- [ ] Review audit logs for suspicious activity.
- [ ] Maintain security documentation.

## 6. Expected Security Improvements

| Security Area | Expected Improvement |
|---|---|
| Authentication | Prevent unauthorized account access |
| Authorization | Restrict access based on user roles |
| Confidentiality | Protect sensitive student information |
| Integrity | Prevent unauthorized data modification |
| Availability | Improve application reliability |
| Accountability | Maintain records of important actions |

## 7. Conclusion

The proposed hardening checklist provides a structured approach to improving student portal security.

Implementing critical and high-priority controls first will help reduce the most significant identified risks.

Continuous monitoring, maintenance and periodic security reviews are also necessary to maintain a secure application.
