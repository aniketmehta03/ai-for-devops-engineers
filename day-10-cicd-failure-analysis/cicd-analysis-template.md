# CI/CD Failure Analysis Template

# Incident Title

Example:

GitHub Actions Deployment Failure

---

# Environment

* Repository:
* Branch:
* Workflow:
* Runner:
* Cloud Provider:

---

# Executive Summary

Brief summary of the failure.

---

# Failed Stage

Examples:

* Build
* Test
* Docker
* Deploy

---

# Error Details

Include:

* Error message
* Timestamp
* Relevant logs

---

# Possible Root Cause

Examples:

* Dependency issue
* Configuration error
* Authentication failure
* Infrastructure problem

---

# Evidence

Supporting logs:

* Log snippet
* Pipeline step
* Exit code

---

# Verification Steps

* Review workflow YAML
* Validate secrets
* Check environment variables
* Re-run failed stage
* Verify infrastructure state

---

# Resolution

Describe how the issue was resolved.

---

# Prevention

* Add validation checks
* Improve testing
* Enhance monitoring
* Update documentation

---

# Lessons Learned

Document improvements for future deployments.

---

# Golden Rule

AI may identify probable causes.

Engineers must validate findings before implementing fixes.

