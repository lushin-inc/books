STUDY LIBRARY
=============

A single-page site that holds your book study companions. Two ways in:
  • By book  — each book opens a page with its four deliverables as tiles.
  • By type  — all Spoken Companions together, all Concept Atlases together, etc.

The four formats are color-coded everywhere:
  Spoken Companion = blue   Insights + Action = amber
  Concept Atlas   = green   Atlas Audio      = purple


ADD A BOOK  (this is the only thing you ever edit)
--------------------------------------------------
1. Make a folder inside /files named with the book's slug, e.g.
        files/atomic-habits/

2. Drop the four files in it, named EXACTLY:
        spoken.docx     Spoken Companion   (Word / Speechify)
        insights.pdf    Insights + Action Guide
        images.pdf      Concept Atlas      (images only)
        audio.pdf       Atlas Audio Companion  (Speechify)
   Optional:
        cover.jpg       a cover image for the book tile

3. Open index.html and add ONE line to the BOOKS list near the top:
        { slug:"atomic-habits", title:"Atomic Habits", author:"James Clear", tags:["Habits","Mindset"] },

That's it. The Topics list in the sidebar builds itself from the tags you use.

Flags you can add to a book line:
   missing:["audio"]   — mark a file that isn't built yet (tile shows it greyed)
   cover:true          — you added a cover.jpg to that book's folder

Rules for slugs: lowercase letters, numbers, and hyphens only, no spaces,
and the slug must match the folder name in /files.


CHANGE A FORMAT'S NAME OR COLOR
-------------------------------
Edit the TYPES block just below the BOOKS list. You rarely need to.


PUBLISH TO GITHUB PAGES
-----------------------
1. Put this whole folder in a GitHub repo (index.html must be at the root).
2. Repo → Settings → Pages → Deploy from a branch → main → /(root) → Save.
3. Your library is live at  https://<your-username>.github.io/<repo>/

To update: replace the file you changed and re-upload. Adding books never
requires touching anything except the BOOKS list and the /files folder.


NOTES
-----
• The 14 seeded books are a starter catalogue with sensible tags — edit,
  delete, or add freely. Each book's file folder is already created for you
  in /files, waiting for you to drop the four files in.
• Fonts load from Google Fonts; everything else is self-contained and uses
  relative links, so it works from any folder or host.
