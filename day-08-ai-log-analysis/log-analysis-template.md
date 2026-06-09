# Log Analysis Template

# Incident Title

Example:

Application Crash During Deployment

---

# Environment

* Cloud Provider:
* Kubernetes Cluster:
* Application:
* Namespace:

---

# Log Summary

Provide a short overview of the logs.

---

# Key Errors

List important error messages.

Example:

* Connection timeout
* Authentication failed
* Container exited with code 1

---

# Possible Root Causes

* Configuration issue
* Network issue
* Application bug
* Resource limitation

---

# Evidence

Supporting log entries:

* Error:
* Timestamp:
* Component:

---

# Verification Steps

Examples:

* Review pod logs
* Check events
* Validate ConfigMaps
* Verify Secrets
* Review deployment

---

# Resolution

Describe the implemented fix.

---

# Rollback Strategy

If fix fails:

* Rollback deployment
* Restore previous configuration
* Validate application health

---

# Monitoring Recommendations

Monitor:

* Error rate
* Pod restarts
* CPU
* Memory
* Response time

---

# Prevention

* Improve alerting
* Add health checks
* Validate configuration before deployment
* Update runbooks

---

# Lessons Learned

Document improvements for future incidents.

