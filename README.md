# fieldwright.dev

Static one-page site for **Field Wright** — the studio name for the field-services
software built by Hunter Easterling (telecom, utilities, property, oilfield).

Single self-contained `index.html` (no build step, no dependencies), hosted on
GitHub Pages at the apex domain `fieldwright.dev`.

## Editing

- **App cards / copy:** edit the `<section id="work">` cards and hero text in `index.html`.
- **Contact:** `contact@fieldwright.dev` (update the `mailto:` links if it changes).

## DNS (apex domain)

`fieldwright.dev` is an apex domain, so it uses **A records** (not a CNAME) pointing at
GitHub Pages:

```
A  @  185.199.108.153
A  @  185.199.109.153
A  @  185.199.110.153
A  @  185.199.111.153
CNAME  www  4easterling.github.io
```

Keep the Cloudflare proxy **off (grey cloud / DNS only)** so GitHub can issue the TLS cert.
