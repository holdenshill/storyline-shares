# storyline-shares

Storyline Creative shared documents, served at https://share.storylinecreative.co.

## Publishing

Vercel hosts this static site in the `storylinecreative/storyline-shares` project. This repository is connected to that project; pushes to `main` deploy to production. GitHub is the source repository, and GitHub Pages build status is not the publishing status for this site.

Each document lives at `<slug>/index.html`, with its optional PDF in the same folder. Keep existing folder names and download filenames so client links continue to work. Commit only the files for the document being updated, push to `main`, and verify the exact public URL and PDF download.

For a manual deployment from a complete checkout, run:

```sh
vercel link --project storyline-shares --scope storylinecreative
vercel deploy --prod --scope storylinecreative
```

The `share` subdomain belongs to this Vercel project. Other Storyline Creative DNS records and email routing are independent of this site.
