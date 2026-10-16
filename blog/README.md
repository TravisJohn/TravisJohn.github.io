# How to add a blog post

For LinkedIn Manager (and anyone publishing a post). No coding knowledge needed beyond careful copying and pasting. Work in the GitHub web UI at https://github.com/TravisJohn/TravisJohn.github.io unless you are told otherwise.

One post = one new file in `blog/posts/`, plus one new entry at the top of `blog/index.html`.

## Steps

1. **Pick the file name.** Use the date and a few words from the title, joined with hyphens, all lower-case. Example: `2026-10-18-my-first-note.html`
2. **Copy the template.** In the repo, open `blog/posts/POST-TEMPLATE.html`, copy the whole file, and create a new file in `blog/posts/` with your file name from step 1. In the GitHub web UI: open the template, click the pencil/copy the text, go to `blog/posts/`, click **Add file → Create new file**, type the file name, and paste.
3. **Fill in the top of the file.** Replace every `[bracketed]` placeholder:
   - `[Post title]` — the post title (it appears twice: browser title and Open Graph title).
   - `[One-sentence summary ...]` — one plain sentence about the post (appears twice).
   - `[YYYY-MM-DD-short-title]` — your file name without `.html` (appears twice, inside the two travisjohn.github.io links).
   - `[YYYY-MM-DD]` — the post date, e.g. `2026-10-18`.
   - `[DD Month YYYY]` — the same date written out, e.g. `18 October 2026`.
4. **Write the body.** Replace `[First paragraph.]` and the other bracketed paragraphs with the post text. Keep one paragraph inside each `<p>...</p>`. For a list, copy this shape: `<ul><li>Point one</li><li>Point two</li></ul>`. Do not delete any lines that start with `<` unless the template comments say you can.
5. **Link it from the blog listing.** Open `blog/index.html`. Find the comment `Newest posts go at the top of this list.` Copy the whole existing `<li>...</li>` block for the Welcome post, paste it directly below that comment (so the newest post is first), then in the pasted copy change: the date in `datetime="..."`, the written date, the title (twice), the one-sentence summary, and both `posts/...html` links to your new file name.
6. **(Optional) Feature it on the home page.** In the root `index.html`, the Blog section shows one post card. If this post should be featured, update that card's date, title, summary and `blog/posts/...html` link in the same way.
7. **Commit.** Use a clear commit message, e.g. `Add blog post: [Post title]`. Commit to `main`.
8. **Check it live.** Wait a minute or two, then open https://travisjohn.github.io/blog/ , click the new post, and check the title, date and paragraphs look right on desktop and phone. Fix mistakes by editing the same files again.

## Rules — do not break these

- Never publish a phone number or street address anywhere on the site.
- Only state career facts that are already on this site or in Travis's CVs. If unsure about a claim, leave it out and ask Travis.
- WooliesX title is **Senior BI Developer, Oct 2021 – Present**. Never use an "8M+ members" figure. Safe Rewards app figure: about 2.4M MAU.
- Do not call Crop Smart a startup. AWS is training-level only — never claim production AWS. No Matillion. "Copilot" means GitHub Copilot.
- Do not rename or delete `POST-TEMPLATE.html`, `blog/index.html`, or existing post files.
- File names: lower-case letters, numbers and hyphens only, starting with the date (`YYYY-MM-DD-...`).
