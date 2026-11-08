<p>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="hero-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="hero.png">
  <img src="hero.png" width="830" alt="tools and infra for the agentic era. fast, secure and reliable.">
</picture>
</p>

Open-source tools and infrastructure for agents, developers and security teams, all in Rust.

Agents now write code, run commands and hold credentials on real machines, but most of the tools around them were built for one person at a keyboard. Whiteheap builds tools for that shift.

We want absolute excellence in software. Each tool leaves your work alone whenever it cannot tell what is safe to touch, and says what it did in a few words. It uses as little CPU and memory as it can, and we measure both on each code change before it ships. Each tool is one Rust binary with as few dependencies as we can manage, and every release carries SHA-256 checksums and a build-provenance attestation.

## Tools

### [residue](https://github.com/whiteheap/residue)

<p>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/whiteheap/residue/main/docs/assets/hero-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/whiteheap/residue/main/docs/assets/hero.png">
  <img src="https://raw.githubusercontent.com/whiteheap/residue/main/docs/assets/hero.png" width="830" alt="Reclaim your storage from Git worktrees, automatically and safely.">
</picture>
</p>

**residue removes a worktree only when nothing in it would be lost, whichever coding agent left it.**

It runs on macOS, Linux and FreeBSD, and comes with a Mac app. The install script installs residue and, on macOS and Linux, turns on automatic cleanup:

```sh
curl -fsSL https://residue.whiteheap.com/install.sh | sh
```

Homebrew alone installs residue without automatic cleanup: `brew install whiteheap/tap/residue`.

The Mac app, shown with example repositories and a made-up history of removals:

<p>
<img src="https://raw.githubusercontent.com/whiteheap/residue/main/docs/screenshots/worktrees.png" width="830" alt="The Worktrees screen: a line that says automatic cleanup freed about 70.3 MB, 1 worktree, since the app was last open, with a link to Freed. Below it, 1.3 GB reclaimable, 6 of 11 worktrees can go, about 975 MB freed in the last 7 days. A treemap sizes each worktree by the space removing it frees, grouped by repository: white for can go, gray for kept, hatched for unknown. Below it, each worktree's checks and verdict.">
</p>

<p>
<img src="https://raw.githubusercontent.com/whiteheap/residue/main/docs/screenshots/freed.png" width="830" alt="The Freed screen: 975 MB freed in the last 7 days, 2.1 GB in the last 30, 5.9 GB all time and 215 MB since the app was last open, a column for each of the last 12 weeks, the space each command freed (residue watch, residue remove --all and residue remove by hand), and the space freed in each repository, most first.">
</p>

Website: [residue.whiteheap.com](https://residue.whiteheap.com) · Source: [github.com/whiteheap/residue](https://github.com/whiteheap/residue)

## The name

Whiteheap joins white hat and heap. A white hat is a hacker who finds weaknesses so they can be fixed, and works in the open. The heap is the memory a program asks for while it runs.
