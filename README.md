# Privacy Documents

> Markdown templates for **Privacy Policy**, **Cookie Policy**, and **Cookie Settings** pages.

## Supported Langues

* `English`

## Variables

To have reusable `Markdown` pages, these template files support variables.

## Usage

 * Install [`predown`](https://github.com/sbstjn/predown)
 * Create TOML configuration (see [`config/example.toml`](config/example.toml))
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

See [`config/example.toml`](config/example.toml) for an example of the full configuration set.
