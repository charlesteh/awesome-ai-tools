# Maintainer workflow

## "validate" command

When the maintainer says just "validate" or "VALIDATE", review every open PR **and** every open issue in charlesteh/awesome-ai-tools, then act without asking:

1. **Check each submission:**
   - It must be an AI tool (AI is part of what it does, per its description or site).
   - It must not already be in `readme.md` (search by name and domain).
   - A PR must only add list line(s) to `readme.md` in the format `- [Name](url) - description`, under a fitting section, with no stray blank lines or unrelated edits.
2. **Accept:**
   - PRs: approve, then squash-merge. If it has a merge conflict or a small formatting problem, add the line yourself through a PR from the working branch, merge that, and close the original PR with a comment linking to it.
   - Issues: add the tool to the right section (use the submitter's suggested line when given), merge through a PR whose body says `closes #N`, and confirm the issues closed.
3. **Reject** (not an AI tool, duplicate, spam, or broken/unsafe link): leave a short comment saying why, then close it. PRs get a REQUEST_CHANGES review before closing.
4. **Report back** with a table: number, tool, verdict, and reason.
