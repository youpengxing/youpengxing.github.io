# Personal Academic Website

A dependency-free, single-page academic homepage written in English. The layout
is intentionally plain: a white page, one narrow column, body paragraphs, one
short program note, and a numbered list of publications and preprints.

The page is static HTML. Every paragraph and publication is present in the
served HTML, so search engines can read it without executing JavaScript.

## File Structure

```text
personal-website/
|-- index.html      Page content and search metadata
|-- styles.css      Minimal typography and spacing
|-- favicon.svg     Minimal browser icon
|-- robots.txt      Search-crawler instructions
|-- sitemap.xml     Search-engine sitemap
`-- README.md
```

## Before Publishing

The profile information and final public URL are already populated in the
site files. The public URL is:

```text
https://youpengxing.github.io/
```

The remaining content step is to replace the publication note in `index.html`
with the final publication list, including collaborators, journals, years, and
links.

Use the final public URL consistently. A matching canonical URL prevents search
engines from treating copies of the page as separate pages.

## Publish With GitHub Pages

1. Create a public GitHub repository named exactly `youpengxing.github.io`.
2. Upload the contents of this `personal-website/` directory to the repository
   root.
3. In the repository, open Settings, then Pages.
4. Under Build and deployment, choose Deploy from a branch.
5. Select the `main` branch and the `/ (root)` directory, then save.
6. The public address is `https://youpengxing.github.io/`.

No server, database, or build command is required.

There is no separate setting to mark a repository as the account homepage. The
repository becomes the user site because its name exactly matches
`youpengxing.github.io`.

## Publish With Cloudflare Pages

1. Push this directory to a GitHub or GitLab repository.
2. Create a Cloudflare Pages project and connect the repository.
3. Choose no framework preset.
4. Leave the build command empty.
5. Use `/` as the output directory.

Cloudflare will provide a public `pages.dev` address. A custom domain can be
connected later in the Cloudflare dashboard.

## Submit To Google Search

1. Confirm that the public website opens in a normal browser.
2. Open Google Search Console and add a Domain property or URL-prefix property.
3. Follow the verification instructions shown by Google.
4. Submit `https://youpengxing.github.io/sitemap.xml` in the Sitemaps section.
5. Use URL Inspection for the homepage and request indexing.

Indexing is not instantaneous. Google may take several days or longer to crawl,
process, and display a new personal website.

## Updating The Site

Edit the text directly in `index.html`. After an update, upload the changed file
again or push it to the connected Git repository. There is no compile step.
