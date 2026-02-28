# <p align="center">2929 Domains - Free Subdomains</p>
**<p align="center">Register your free subdomains!</p>**

<p align="center">
    <img src="https://img.shields.io/github/stars/2929-domains/registry?label=Stars&style=for-the-badge&color=FFD700" alt="Stars">&nbsp;&nbsp;
    <img src="https://img.shields.io/github/directory-file-count/2929-domains/registry/records?label=Records&style=for-the-badge&color=4CAF50" alt="Users">&nbsp;&nbsp;
    <img src="https://img.shields.io/github/issues-pr/2929-domains/registry?label=PRs&style=for-the-badge&color=FFA500" alt="Pull Requests">
</p>


## How to Register

1. Fork this repository.  
2. Read the full [DOCS.md](./DOCS.md) for instructions and rules.  
3. Create a folder in `/records` named after your GitHub username
4. Inside your folder, create a JSON file for your subdomain (e.g., `myproject.json`).  
5. Complete the JSON fields as instructed below.  
6. Open a pull request — automated checks will validate your submission.  
7. Once approved, your subdomain will become active.

> Automated validation ensures JSON and subdomain rules are correct, but all PRs undergo review before activation.


## Supported DNS Record Types

- **A**, **AAAA**, **CNAME**, **TXT**


## JSON Template

Place your JSON file in your folder and follow this structure:

```json
{
"githubUname": "yourGitHubUsername",
"publicEmail": "your-email@example.com",
"desc": "Short description of your subdomain",
"domain": "029290.xyz",
"subDomain": "desired-subdomain",
"records": [
 { "name": "@", "type": "CNAME", "value": "example.github.io", "proxied": "true" },
 { "name": "panel", "type": "CNAME", "value": "panel.example.io", "proxied": "true" }
]
}
```
> Ensure subDomain is unique and follows rules in DOCS.md.


## Notes

Users can only manage files inside their own folder.

Reserved subdomains cannot be registered at the root level.

Blocked subdomains cannot be used at any level.

Keep JSON valid — no trailing commas.



## License

This project is licensed under the MIT License. See LICENSE for details.



## Contact

For support, open an issue in this repository.
