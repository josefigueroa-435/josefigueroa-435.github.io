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

- [x] LinkedIn and Handshake links are in.
- [ ] Confirm the Handshake public profile is switched on (profile icon → Settings),
      otherwise that link asks visitors to log in.
- [x] Phone: the resume PDF and the pages both carry the Google Voice job-search
      number (760) 299-5082, not the personal line. Safe to publish.
- [x] GitHub account name decided: `josefigueroa-435`. Rename the existing account
      under Settings → Account → Change username before publishing, or the links on
      every page will 404.
- [ ] Optional: add a photo.

The live URL will be **https://josefigueroa-435.github.io**.

## Publishing on GitHub Pages

1. Create a new **public** repository named `josefigueroa-435.github.io`.
2. In GitHub Desktop: File → Add local repository → this folder → Publish.
3. Repository → Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
4. The site appears at `https://josefigueroa-435.github.io` within a minute or two.

Pushing a commit republishes it. There is nothing to build.

## Editing

Colors and fonts are tokens in the `:root` block at the top of `style.css`; the dark
theme redefines the same tokens further down. Changing a token changes every page.

Contact details appear twice: the footer list at the bottom of all four pages, and the
Contact block on `index.html` and `resume.html`. Change a link and you have to change
it in both places.

The phone number on the site is the Google Voice number, which forwards and transcribes.
The personal line never appears here or in the PDF.

Layout: each section is a `.row` — the heading sits in the left margin column, the
content in the right. At narrow widths the heading stacks above its content.
