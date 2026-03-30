# timefyi

[![crates.io](https://img.shields.io/crates/v/timefyi.svg)](https://crates.io/crates/timefyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Timezone operations, business hours, and sunrise/sunset — API client for [timefyi.com](https://timefyi.com).

> **Try the interactive tools at [timefyi.com](https://timefyi.com)**

## Install

`cargo add timefyi`

## Quick Start

```rust
use timefyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("seoul").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install timefyi` | [PyPI](https://pypi.org/project/timefyi/) |
| **npm** | `npm install timefyi` | [npm](https://www.npmjs.com/package/timefyi) |
| **Go** | `go get github.com/fyipedia/timefyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/timefyi-go) |
| **Rust** | `cargo add timefyi` | [crates.io](https://crates.io/crates/timefyi) |
| **Ruby** | `gem install timefyi` | [rubygems](https://rubygems.org/gems/timefyi) |

## Embed Widget

Embed [TimeFYI](https://timefyi.com) widgets on any website with [timefyi-embed](https://widget.timefyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/timefyi-embed@1/dist/embed.min.js"></script>
<div data-timefyi="entity" data-slug="seoul"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.timefyi.com)

## Links

- [TimeFYI](https://timefyi.com) — Main site
- [API Documentation](https://timefyi.com/developers/)
- [OpenAPI Spec](https://timefyi.com/api/openapi.json)
- [Glossary](https://timefyi.com/glossary/)

## License

MIT
