# Jose Figueroa — personal site

Static site, no build step. Four pages plus one stylesheet.

```
index.html      About / home
research.html   Research
projects.html   Projects
resume.html     Resume (HTML) + PDF download
style.css       All styling (design tokens live in :root at the top)
Jose-Figueroa-Resume.pdf
```

## Before it goes live

- [ ] Replace `LINKEDIN-URL-HERE` in all four HTML files with the real LinkedIn URL.
- [ ] Replace the `Jose-Figueroa-Resume.pdf` with a web copy that has the phone number removed.
- [ ] Decide on the GitHub account name — it appears in the GitHub link on every page
      and in the site's own URL.
- [ ] Optional: add a photo to the identity panel.

## Publishing on GitHub Pages

1. Create a new **public** repository named `<username>.github.io`.
2. In GitHub Desktop: File → Add local repository → this folder → Publish.
3. Repository → Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
4. The site appears at `https://<username>.github.io` within a minute or two.

Pushing a commit republishes it. There is nothing to build.

## Editing

Colors and fonts are tokens in the `:root` block at the top of `style.css`; the dark
theme redefines the same tokens further down. Changing a token changes every page.

The contact panel on the left is the same block of HTML in all four pages — edit it in
one and copy it to the other three.
