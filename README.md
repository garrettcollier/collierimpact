# Collier Impact

A responsive, dependency-free informational website for an impact fund in development. Near-black backgrounds, bold upright typography, copper accents, original structural artwork, and accessible research accordions. Includes the founding Mission, North Star, and investment principles.

## Local preview

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

Open <http://127.0.0.1:4173>. No installation or build is required. Refresh after edits.

## Editing

- `index.html`: public copy and contact links.
- `assets/site.css`: typography, layout, colors, and responsive styles.
- `assets/site.js`: mobile menu, section highlighting, and reduced-motion-aware reveals.
- `assets/connected-systems.svg`: original abstract artwork, not a project photograph.
- `assets/social-card.png`: social preview.
- `privacy.html`, `404.html`, `robots.txt`, `sitemap.xml`: supporting pages and metadata.

Email links use `garrettcollierbusiness@gmail.com`. Change all occurrences when updating the contact address. The site has no analytics, forms, external fonts, or runtime dependencies. Update the privacy copy if that changes.

## GitHub Pages

The included workflow publishes public site files when reviewed changes are pushed to `main`, or when manually dispatched. Repository internals and this README are excluded.

1. Choose **GitHub Actions** in this repository's **Settings → Pages**.
2. Push reviewed changes to `main` and check the deployment workflow.
3. Verify ownership in your GitHub account's Pages settings; set the repository custom domain to `collierimpact.com` before changing DNS.
4. Configure these registrar records while preserving unrelated email and verification records:

| Type | Host | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `garrettcollier.github.io` |

Replace conflicting parking or forwarding records at those hosts. After domain checks and certificate provisioning succeed, enable **Enforce HTTPS**. Do not use wildcard DNS.

The `CNAME` file also supports branch-based publication. With the included Actions workflow, configure the domain in repository settings; the file alone does not configure it.

Sources checked November 16, 2026: [GitHub custom-domain guidance](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site), [official static workflow](https://github.com/actions/starter-workflows/blob/main/pages/static.yml).

## Public positioning

The website presents a founding-stage impact fund, not a live investment offering. All six research areas are exploratory, with no selected launch sector. No track record, assets under management, active investment team, or realized outcomes are claimed. Internal founding documents and personal compensation targets are not published.
