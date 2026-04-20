# Vault Hub Blog

Source of truth for posts published at https://obsidianvaulthub.com/blog.

## Writing a post

1. Drop a new `.md` file in this folder.
2. Add frontmatter:

   ```yaml
   ---
   title: Post Title
   date: 2026-04-20
   summary: One-line summary for the index page.
   tags: [tag1, tag2]
   ---
   ```

3. Commit and push:

   ```bash
   git add .
   git commit -m "post: <slug>"
   git push
   ```

The slug is the filename minus `.md`. The site's `/blog` route revalidates every 60s, so new posts show up within a minute without a redeploy.
