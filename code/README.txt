Put the ZIP archive of your source code here.

The project page offers your code as a direct ZIP download - it does
NOT link to a repository.

Rules:
- One ZIP file, e.g. lastname-project-code.zip
- HARD LIMIT: under 100 MB (GitHub rejects larger files)
- No secrets: remove API keys, tokens, .env files, credentials
- No bulky build artifacts (node_modules, venv, dist/, caches)
- Include a README and license information inside the archive
- The archive must match your submission state

Export a clean snapshot from your code repository (run inside it):

  git archive --format=zip \
      -o ../<your-page-repo>/code/lastname-project-code.zip submission

git archive exports the tagged state WITHOUT the .git folder - right
for the public download. The graded hand-in ZIP including .git is a
separate deliverable (see the Thesis Guide, Section 6).

Then check both links in index.html (header button + Source Code
section) point to your file.
