# Gears & Grooves

**Wrenches by day, beats by night.** The blog at gearsandgrooves.com.

Built with Eleventy, edited with Pages CMS, and hosted on Cloudflare Pages. It's the same setup as manymanytoes.com.

## What's inside

```
src/
  _data/site.json        site title, tagline, music/social links
  _data/categories.json  Gears, Grooves, Engineering Life, Kuya Talk
  _includes/             page layouts
  posts/                 blog posts (Markdown)
  uploads/               images added through the CMS
  assets/img/logo.svg    G&G logo
  index.njk              homepage
  about.md               About page
.pages.yml               Pages CMS setup
```

## Going live

1. **GitHub:** create a new repo (e.g. `gearsandgrooves`) and upload everything in this folder.
2. **Cloudflare Pages:** go to Workers & Pages, then Create, then Pages, then Connect to Git, and pick the repo.
   - Framework preset: **Eleventy**
   - Build command: `npx @11ty/eleventy`
   - Build output directory: `_site`
   - Environment variable: `NODE_VERSION` = `22`
3. **Domain:** in the Pages project, open Custom domains and add `gearsandgrooves.com` (and `www`).
4. **CMS:** sign in at app.pagescms.org with GitHub and open the repo. Posts and Site settings will show up in the sidebar.

## Writing a post

In Pages CMS, go to Posts, then Add an entry. Fill in the title, date, category, tags, a short summary, an optional cover image, and the body. Save it and Cloudflare rebuilds the site in about a minute.

The four sample posts are placeholders, so edit or delete them.

## Music links

Open Site settings in the CMS and paste his Spotify, YouTube, or Instagram links. They appear in the footer automatically. To embed a track in a post, paste the Spotify or YouTube embed code into the body.

## Running it locally (optional)

```
npm install
npm start
```

Then open http://localhost:8080.
