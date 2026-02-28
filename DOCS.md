# Documentation

Welcome to the **029290.xyz free subdomain service**. This document provides **rules, structure, and guidelines** for contributing to the repository and registering subdomains under the 029290.xyz.

---

## 1. Repository Structure

Each user has a personal folder inside `/records/`:

```
/records/<github-username>/
```

**Each subdomain requires a separate JSON file** inside your folder.

- Users can create, edit, update, and delete files **only inside their own folder**.
- Files cannot be added or modified outside your own folder.
- All files must be **valid JSON**:

```json
{
  "githubUname": "",
  "publicEmail": "",
  "desc": "",
  "subDomain": "",
  "records": [
    { "name": "", "type": "A|AAAA|CNAME|TXT", "value": "", "proxied": "true|false" }
  ]
}
```

**Required fields**: `githubUname`, `publicEmail`, `desc`, `subDomain`, `records`.  
**Allowed DNS types**: A, AAAA, CNAME, TXT.

---

## 2. Reserved Subdomains

Root-level reserved (cannot register directly):

- `admin.029290.xyz`
- `www.029290.xyz`
- `dashboard.029290.xyz`

**Allowed as sub-subdomains**:
- ✅ `admin.user.029290.xyz`
- ❌ `admin.029290.xyz`

List in `reserved.txt` (supports `*` wildcards).

---

## 3. Blocked Subdomains

Cannot register at any level. Full list in `blocked.txt` (supports `*`).

---

## 4. Protected Files

Cannot edit/delete:

- `LICENSE.md`
- `README.md`
- `DOCS.md`
- `CONTRIBUTING.md`
- `.github/workflows/*`

---

## 5. Pull Request Guidelines

All changes via PRs. Auto-validation:

1. Your folder only
2. JSON structure
3. Reserved/blocked rules

**Fails = no merge.** Fork-safe.

---

## 6. Naming Conventions

- camelCase JSON keys
- lowercase subdomains
- No trademarks/offensive names

---

## 7. Best Practices

- Test JSON locally
- Check conflicts
- Clear `desc`
- Minimal records
- One subdomain per file

---

Secure, fair, maintainable free subdomains under 029290.xyz.
