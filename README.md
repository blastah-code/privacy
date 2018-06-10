# Privacy Documents

> Markdown templates for **Privacy Policy**, **Cookie Policy**, and **Cookie Settings** pages.

## Supported Langues

* `English`

## Variables

To have reusable `Markdown` pages, these template files support variables.

## Usage

 * Install `[predown]`
 * Create TOML configuration (see `config/example.toml`)
 * Download Markdown sources (aka fork this repository)

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

See `config/example.toml` for an example of the full configuration set:

```toml
[Contact]

Address = "Lorem Ipsum\n126 Silver Maple Ave\nCle Elum, Washington (WA), 98922"
Phone = "+1-202-555-0111"
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

[predown]: https://github.com/sbstjn/predown