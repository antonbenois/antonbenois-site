# Anton Benois — static website starter

This folder is a plain HTML/CSS website. There is:

- no Wix
- no WordPress
- no database
- no build process
- no npm
- no paid hosting requirement

You can open `index.html` directly in a browser.

## Folder structure

- `index.html` — homepage / work index
- `bio/index.html` — About / CV
- `contact/index.html` — contact page
- `project-template/index.html` — duplicate this folder for each project
- `assets/css/site.css` — appearance for the whole website
- `assets/images/` — put your images here

## Making a project page

1. Duplicate `project-template`.
2. Rename the copy, e.g.:
   `living-objects`
3. Edit `living-objects/index.html`.
4. Put its images in:
   `assets/images/living-objects/`
5. Replace placeholders with normal image elements, for example:

   <img src="../assets/images/living-objects/01.jpg"
        alt="Installation view of Living Objects">

6. On the homepage, change the project's link to:
   `living-objects/`

That produces:
`antonbenois.com/living-objects/`

## Images

Do not use your huge print originals directly.

A sensible starting point for web:
- JPEG or WebP
- about 2000–3000 px on the long edge for normal documentation
- usually under 1 MB per image when possible
- keep the original archive files elsewhere

## Previewing

The simplest method:
double-click `index.html`.

For a more accurate local preview, if Python is installed:

    cd antonbenois-site-starter
    python3 -m http.server 8000

Then visit:
http://localhost:8000

## Publishing with GitHub Pages later

Nothing needs to be done today.

When ready:

1. Create a GitHub account/repository if needed.
2. Upload the contents of this folder.
3. Enable GitHub Pages for the repository.
4. Confirm the temporary GitHub Pages URL works.
5. In GitHub Pages settings, add the custom domain:
   `www.antonbenois.com` or `antonbenois.com`
6. Only after the new site is working, change the DNS records at Namecheap.
7. Keep Wix alive until the custom domain works correctly.
8. Cancel Wix before renewal.

We can do the DNS change together. Do not change Namecheap nameservers or delete Wix DNS records prematurely.

## What to do this weekend

Recommended order:

1. Decide which projects actually belong on the 2026 homepage.
2. Gather one homepage image for each.
3. Gather the images for ONE project.
4. Build that project from `project-template`.
5. Adjust typography/image scale until that one page feels right.
6. Only then duplicate it for the rest.
7. Copy/edit your About/CV last.

Avoid spending hours migrating obsolete pages before deciding whether they should survive.

## Important

Keep your domain registered at Namecheap.

Hosting and domain registration are separate things. Moving the site off Wix does not require transferring the domain away from Namecheap.


## First real project: Lost in Space

The homepage now links to `lost-in-space/index.html`.

Put selected images into:

`assets/images/lost-in-space/`

Then replace each placeholder with an image tag, e.g.:

    <img src="../assets/images/lost-in-space/01.jpg"
         alt="Lost in Space, artist book, 2026">

Start with 6–10 strong images rather than migrating every image automatically.


## Portrait documentation rule

Portrait images do not expand to full project-page width.

- Two related portraits: wrap the two figures in `<div class="portrait-pair">`.
- One portrait: use `<figure class="portrait-single">`.
- Desktop single portraits are roughly one-third of available width.
- Mobile rules enlarge them enough to remain readable.


## Current project set

The homepage currently contains the post-MFA sequence:

- Lost in Space, 2026
- Ingenmannsland, 2026
- Archive, 2026
- End of History Part 1, 2023
- Living Objects, 2021
- Mutations, 2021
- Permanent Vacation, 2020
- Distant Relatives, 2019

`Archive` is the final public title for the installation previously developed under the working title `Page Bodies`.
