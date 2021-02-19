# Desired State Checklist: GIT Repositories

* I like a `readme.md` that provides:
  * What the software is, does, and why
  * Maintainer contact information
  * Instructions on how to build, run, and test the project
* I like having all developer/supporter documentation in the repo as markdown files.
* I like a `.gitginore` that excludes:
  * Artifacts that may get generated on either Mac OS or Windows
  * IDE support files
  * Operating system cruft (.ds_store, thumbs.db, etc)
* I like an `.editorconfig` file that:
  * Enforces character sets
  * Let’s me forget about tab vs spaces and indent sizes
  * Minimizes noise in commit deltas (whitespace changes)
* I like a `.gitattributes` that:
  * Enforces EOL characters and character sets
  * Treats goldenfiles and testdata as binary
* I like being able to run a linter against the project using a Docker container.
* I dislike active projects that don’t have their documentation periodically audited and updated.
* I like non-trivial repos that include a [architecture.md](https://matklad.github.io//2021/02/06/ARCHITECTURE.md.html) ([archive link](https://archive.is/bsIbE)).
