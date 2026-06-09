# Li Jionghui Calvin Portfolio

Static bilingual portfolio website for GitHub Pages.

## GitHub Pages Setup

1. Open this repository on GitHub.
2. Go to `Settings > Pages`.
3. Set source to `Deploy from a branch`.
4. Select branch `main` and folder `/root`.
5. Save.

The custom domain is configured in `CNAME`:

```text
calvin-88.com
```

## DNS Setup For `calvin-88.com`

At your domain registrar, add GitHub Pages DNS records:

```text
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
CNAME www   cocodsr-jpg.github.io
```

After DNS is saved, return to GitHub Pages settings and enable `Enforce HTTPS`.

## Local Preview

```powershell
python -m http.server 8080 --bind 127.0.0.1
```

Then open `http://127.0.0.1:8080/`.
