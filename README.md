### How to Remove Branches

**Locally:**
```bash
git branch -d <branch_name>
git push origin --delete <branch_name>

### Annotated Tags vs Lightweight Tags

- **Annotated Tags:** Contain a message, metadata (tagger name, email, date), and are stored as full objects in Git history.
- **Lightweight Tags:** Are pointers to a specific commit, with no additional metadata.

**Use Annotated Tags** for releases and significant milestones. Use lightweight tags for quick, local references.

### When to Use Rebase

Use rebase to:
- Keep a linear commit history.
- Incorporate changes from one branch into another without creating a merge commit.

Example:
```bash
git checkout feature-branch
git rebase main

### How to List Tags

To list all tags:
```bash
git tag

### How to Delete a Tag Locally and Remotely

**Locally:**
```bash
git tag -d <tag_name>
git push origin --delete <tag_name>
