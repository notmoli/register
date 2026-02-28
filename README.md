<p align="center">
  <h1 align="center">2929-domains</h1>
</p>

<p align="center">

  <img src="https://img.shields.io/github/contributors/2929-domains/register" alt="Contributors" />
  <img src="https://img.shields.io/github/issues/2929-domains/register" alt="Issues" />
  <img src="https://img.shields.io/github/license/2929-domains/register" alt="License" />
</p>

---

<p align="center">
2929-domains is a free subdomain registration platform for students and those who just want to get experience of domains.
It allows users to register subdomains under domain like <code>029290.xyz</code>, manage DNS records, and ensure uniqueness.
</p>

---

<h2 align="center">Domain List</h2>

<p align="center">Currently available domains for registration:</p>

<ul>
  <li><code>029290.xyz</code></li>
  <li>More coming soon…</li>
</ul>

<p><em>Stay tuned! We will expand the list as the project grows.</em></p>

---

<h2 align="center">Features</h2>

<ul>
  <li>Users can create, update, and delete <strong>their own subdomain records</strong>.</li>
  <li>Protected and workflow files cannot be edited.</li>
  <li>Validates JSON files with required fields: <code>githubUname</code>, <code>publicEmail</code>, <code>desc</code>, <code>domain</code>, <code>subDomain</code>, <code>records</code>.</li>
  <li>Checks <code>records</code> array and ensures valid DNS types (<code>A</code>, <code>AAAA</code>, <code>CNAME</code>, <code>TXT</code>).</li>
  <li>Reserved subdomains cannot be registered at root level.</li>
  <li>Blocked subdomains cannot be registered at any level.</li>
  <li>Automatic checks prevent PRs with invalid subdomains from being merged.</li>
</ul>

---

<h2 align="center">Getting Started</h2>

<ol>
  <li>Read the <a href="./DOCS.md">DOCS.md</a> for detailed instructions on subdomain registration and JSON structure.</li>
  <li>Fork the repository.</li>
  <li>Create your folder under <code>/records/&lt;github-username&gt;/</code>.</li>
  <li>Add your JSON file(s) following the correct format.</li>
  <li>Open a pull request — the workflow will automatically validate your submission.</li>
</ol>

---

<h2 align="center">JSON Format Example</h2>

<pre><code>{
  "githubUname": "tokisensei",
  "publicEmail": "example@gmail.com",
  "desc": "My test subdomain",
  "domain": "029290.xyz",
  "subDomain": "him",
  "records": [
    { "name": "@", "type": "CNAME", "value": "example.github.io", "proxied": "true" },
    { "name": "panel", "type": "CNAME", "value": "panel.example.io", "proxied": "true" }
  ]
}
</code></pre>

<p><em>⚠️ Ensure your <code>subDomain</code> is unique and follows the rules outlined in <code>DOCS.md</code>.</em></p>

---

<h2 align="center">License</h2>

<p>This project is licensed under the <strong>MIT License</strong>. See the <a href="./LICENSE">LICENSE</a> file for details.</p>

---

<h2 align="center">Contact</h2>

<p>For questions or support, open an issue in this repository.</p>
---

## Features

- Users can create, update, and delete **their own subdomain records**.  
- Protected and workflow files **cannot be edited**.  
- Validates JSON files with required fields: `githubUname`, `publicEmail`, `desc`, `domain`, `subDomain`, `records`.  
- Checks `records` array and ensures valid DNS types (`A`, `AAAA`, `CNAME`, `TXT`).  
- Reserved subdomains cannot be registered at root-level.  
- Blocked subdomains cannot be registered at all.  
- Automatic checks prevent PRs with invalid subdomains from being merged.  

---

## Getting Started

1. **Read the [DOCS.md](./DOCS.md)** for detailed instructions on subdomain registration and JSON structure.  
2. Fork the repository.  
3. Create your folder under `/records/<github-username>/`.  
4. Add your JSON file(s) following the correct format.  
5. Open a pull request — the workflow will automatically validate your submission.  

---

## JSON Format Example

```json
{
  "githubUname": "",
  "publicEmail": "example@gmail.com",
  "desc": "",
  "domain": "029290.xyz",
  "subDomain": "him",
  "records": [
    { "name": "@", "type": "CNAME", "value": "example.github.io", "proxied": "true" },
    { "name": "panel", "type": "CNAME", "value": "panel.example.io", "proxied": "true" }
  ]
}
```
> ⚠️ Ensure your subDomain is unique and follows the rules outlined in DOCS.md.




---

License

This project is licensed under the MIT License. See the LICENSE file for details.


---

Contact

For questions or support, open an issue in this repository.
