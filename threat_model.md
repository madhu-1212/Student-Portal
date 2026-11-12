
flowchart TB
    S[Student]
    A[Administrator]

    subgraph TB1["Trust Boundary 1 - External Users"]
        S
        A
    end

    subgraph TB2["Trust Boundary 2 - Application Environment"]
        W[Student Portal Web Application]
        AUTH[Authentication Module]
        API[Application Server]
    end

    subgraph TB3["Trust Boundary 3 - Data Environment"]
        DB[(Student Database)]
    end

    E[External Email Service]

    S -->|Login and requests| W
    A -->|Admin requests| W
    W --> AUTH
    AUTH --> API
    API -->|Read and write data| DB
    API -->|Send notifications| E

---

# STRIDE Threat Analysis

## 1. Spoofing
**Threat:** An unauthorized person may pretend to be a registered student or administrator using stolen credentials.

**Impact:** Unauthorized account access.

**Recommended Control:**
- Use strong password policies.
- Implement Multi-Factor Authentication (MFA).
- Use secure login sessions.

## 2. Tampering
**Threat:** An unauthorized user may modify student records, marks, or assignment information.

**Impact:** Incorrect academic information and data integrity loss.

**Recommended Control:**
- Implement role-based access control.
- Validate all user inputs.
- Restrict database modification permissions.

## 3. Repudiation
**Threat:** A user may deny performing an important action, such as modifying a student record.

**Impact:** Difficulty investigating security incidents.

**Recommended Control:**
- Maintain audit logs.
- Record important user activities.
- Protect logs from unauthorized modification.

## 4. Information Disclosure
**Threat:** Confidential student information may be exposed to unauthorized users.

**Impact:** Loss of privacy and confidentiality.

**Recommended Control:**
- Use HTTPS.
- Encrypt sensitive information.
- Restrict access to student records.

## 5. Denial of Service
**Threat:** Excessive requests may make the student portal unavailable.

**Impact:** Students and administrators may be unable to access the portal.

**Recommended Control:**
- Implement rate limiting.
- Monitor unusual traffic.
- Use appropriate server resource limits.

## 6. Elevation of Privilege
**Threat:** A student may gain administrator-level permissions due to incorrect authorization checks.

**Impact:** Unauthorized access to administrative functions.

**Recommended Control:**
- Implement Role-Based Access Control (RBAC).
- Verify permissions on the server.
- Follow the principle of least privilege.

