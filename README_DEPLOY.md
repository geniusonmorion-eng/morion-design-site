# Deploy morion.design on GitHub Pages

This folder is an independent static copy of the site prepared for `morion.design`.

## GitHub Pages

1. Put these files in the GitHub Pages publishing source branch/folder.
2. In GitHub, open the repository settings: `Settings` -> `Pages`.
3. Set `Custom domain` to `morion.design`.
4. Enable `Enforce HTTPS` after GitHub finishes issuing the certificate.

## DNS

For the apex domain `morion.design`, add GitHub Pages `A` records:

```text
@  A  185.199.108.153
@  A  185.199.109.153
@  A  185.199.110.153
@  A  185.199.111.153
```

Optional IPv6 records:

```text
@  AAAA  2606:50c0:8000::153
@  AAAA  2606:50c0:8001::153
@  AAAA  2606:50c0:8002::153
@  AAAA  2606:50c0:8003::153
```

If `www.morion.design` is needed too, add a `CNAME` for `www` that points to the repository's default GitHub Pages domain, for example `username.github.io`.
