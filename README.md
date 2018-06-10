# Privacy Documents

> Markdown templates for **Privacy Policy**, **Cookie Policy**, and **Cookie Settings** pages.

## Supported Langues

* `English`

## Variables

To have reusable `Markdown` pages, these template files support variables.

## Usage

 * Install [`predown`](https://github.com/sbstjn/predown)
 * Create TOML configuration file
 * Download latest [GitHub Release](releases)

## Processing

```bash
$ > ./predown build \
    --config ./config/example.toml \
    --templates ./src/en \
    --destination ./dist

Using config file ./config/example.toml
Using templates prefix ./src/en
Using destination path ./dist

Done: src/en/cookies/policy.md -> dist/cookies/policy.md
Done: src/en/cookies/settings.md -> dist/cookies/settings.md
Done: src/en/privacy.md -> dist/privacy.md
````

### Configuration

The current templates support the following configuration:

```toml
[Contact]

Mail = "privacy@example.com"

[Links]

Privacy = "/privacy.html"

[Links.Cookies]

Policy = "/cookies/policy.html"
Settings = "/cookies/settings.html"

[Cookies]

[[Cookies.Necessary]]

Name = "necessary_cookie"
Info = "Description for necessary cookie"
Expires = "1y"

[[Cookies.Functional]]

Name = "functional_cookie"
Info = "Description for functional cookie"
Expires = "10d"

[[Cookies.Performance]]

Name = "performance_cookie"
Info = "Description for performance cookie"
Expires = "100m"
```