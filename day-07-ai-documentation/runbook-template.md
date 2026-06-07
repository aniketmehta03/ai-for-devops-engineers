# Production Runbook Template

# Title

Example:
CrashLoopBackOff Investigation

---

# Overview

Brief description of the issue.

---

# Symptoms

Examples:

* Pod restarting continuously
* Service unavailable
* High error rate

---

# Possible Causes

* Application crash
* Missing environment variable
* Database connection failure
* Invalid configuration
* Resource constraints

---

# Verification Steps

Run:

```bash
kubectl get pods

kubectl describe pod <pod-name>

kubectl logs <pod-name>

kubectl logs <pod-name> --previous
```

Verify:

* Events
* Logs
* ConfigMaps
* Secrets

---

# Resolution Steps

1. Identify root cause

2. Fix configuration

3. Redeploy

4. Validate application

---

# Rollback Strategy

If deployment fails:

* Rollback deployment
* Restore previous version
* Verify service health

---

# Monitoring Recommendations

Monitor:

* Pod Restarts
* CPU
* Memory
* Error Rate
* Response Time

---

# Prevention

* Add health checks
* Improve monitoring
* Validate configurations
* Automate testing

---

# Lessons Learned

Document improvements for future incidents.

