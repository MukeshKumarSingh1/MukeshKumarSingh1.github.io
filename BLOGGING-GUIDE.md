# Publishing a daily journal entry

The journal is one standalone root-level page: `journal.html`. There is no posts directory, CMS, database, framework, or build step.

1. Open `journal.html` in a text editor.
2. Duplicate the `<article>` block inside the `#entries` section.
3. Place the duplicate first, then update its category, date, title, summary, and destination link. For a short daily note, the full entry may be written directly in the card. For a long essay, create a descriptive root-level HTML page and link to it.
4. Move the newest substantial entry into the `#latest` section if it should receive the full editorial treatment.
5. Update the `BlogPosting` data in the page's JSON-LD, the RSS item in `feed.xml`, and the `<lastmod>` value for `journal.html` in `sitemap.xml`.
6. Test from this directory with `python3 -m http.server 8000`, then open `http://localhost:8000/journal.html`.
7. Upload the contents of this directory to the root of your GitHub Pages repository.

Use a unique descriptive heading, an accurate date, useful internal links, and natural subject terminology. Do not repeat keywords mechanically.
