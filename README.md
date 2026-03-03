## 🐛 Bug Story: Vulnerability Found & Fixed

### Discovery
- **Tool**: GitHub Dependabot + Snyk scan
- **Repo**: vigsecure developer-sample-repo
- **Date**: March 2, 2026
- **Alert**: 1 High severity vulnerability detected in `requirements.txt`

### Vulnerability Details


### Root Cause
Outdated urllib3 version (<1.26.18) with known redirect handling flaw.

### Steps to Reproduce
1. Clone repo: `git clone https://github.com/vigsecure/developer-sample-repo`
2. Run `pip install -r requirements.txt`
3. Dependabot/Snyk flags CVE-2021-33503 automatically

### Fix Applied



### Verification
- Updated requirements.txt ✓
- Re-ran Snyk test: Clean scan ✓
- Dependabot alert dismissed ✓
- Security policy blocked risky merge ✓

### Lessons Learned
1. Dependabot catches deps automatically
2. Snyk scans deeper with exploit paths  
3. Security policy prevents bad commits
4. Pin versions but enable auto-updates

**Status**: Fixed ✅ | **Time to Resolve**: 15 minutes
