# Strict Guidelines for AI Agents Working on This Repository

Every AI agent, assistant, or automated tool working on this repository MUST strictly follow these non-negotiable rules:

---

### 1. Git Push Restrictions (STRICT)
- **NEVER push to remote (`git push`) on your own volition.**
- You must **NEVER** assume permission to push or chain `git push` into a commit command.
- Pushing to remote (`origin/master` or any branch) is **STRICTLY PROHIBITED** unless the user gives an explicit, unambiguous command such as *"push it"* or *"git push"*.
- Always keep changes local and let the user inspect them on the local preview first.

### 2. Header & Navigation Integrity (STRICT)
- **NEVER add new links, buttons, badges, or items to the top header navigation** unless explicitly requested by the user.
- The top header navigation menu is strictly reserved for core sections:
  - **Catalogue** (`#products`)
  - **Designs** (`#designs`)
  - **Contact** (`#contact`)
- Utility, policy, and legal pages (such as Privacy Policy) belong strictly in the **footer**, never in the main top navigation.

### 3. Clean URL Routing (No `.html` in public URLs)
- Pages must be served as clean URLs without `.html` extensions.
- Use directory-based structure: create `<page>/index.html` (e.g., `/privacy/index.html`) so that requests to `https://tibrewalaelectricals.com/privacy` resolve directly and cleanly.
- Internal links must point to `privacy` (not `privacy.html`).

### 4. Personal Git Identity & Zero AI/Bot Metadata
- Commits and pushes must **STRICTLY** use the repository's local personal configuration:
  - **Author / Committer**: `Sanket Tantia <19sanket95@gmail.com>`
  - **SSH Key**: `~/.ssh/id_ed25519_personal` with `-o IdentitiesOnly=yes`
- **NEVER** include `Co-authored-by:`, AI signatures, bot tags, or tool watermarks in commit messages.

### 5. Local Verification Before Presentation
- Always verify changes locally on `http://localhost:8000` before declaring work done.
- Do not make speculative or unsolicited aesthetic redesigns beyond what the user asked for.
