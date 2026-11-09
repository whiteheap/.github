<p>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="hero-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="hero.png">
  <img src="hero.png" width="830" alt="tools and infra for the agentic era. fast, secure and reliable.">
</picture>
</p>

Open-source tools and infrastructure for agents, developers and security teams.

Agents now write code, run commands and hold credentials on real machines, but most developer tools were made for a person typing commands, not an agent running them. Whiteheap builds tools for that shift.

We want absolute excellence in software. Our tools never touch your work unless they're sure it's safe, and they tell you what they did in a few words. They're fast and light, and we measure every change that could slow them down. You can check that every release is exactly what we built.

## Tools

### [residue-cli](https://github.com/whiteheap/residue-cli)

<p>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/whiteheap/residue-cli/main/docs/assets/hero-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/whiteheap/residue-cli/main/docs/assets/hero.png">
  <img src="https://raw.githubusercontent.com/whiteheap/residue-cli/main/docs/assets/hero.png" width="830" alt="Reclaim your storage from Git worktrees, automatically and safely.">
</picture>
</p>

**residue removes a worktree only when nothing in it would be lost, whichever coding agent left it.**

It runs on macOS, Linux and FreeBSD. The install script installs residue and, on macOS and Linux, turns on automatic cleanup:

```sh
curl -fsSL https://residue.whiteheap.com/install.sh | sh
```

Homebrew alone installs residue without automatic cleanup: `brew install whiteheap/tap/residue`.

Website: [residue.whiteheap.com](https://residue.whiteheap.com) · Source: [github.com/whiteheap/residue-cli](https://github.com/whiteheap/residue-cli)

### [residue-ui](https://github.com/whiteheap/residue-ui)

<p>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/whiteheap/residue-ui/main/docs/assets/hero-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/whiteheap/residue-ui/main/docs/assets/hero.png">
  <img src="https://raw.githubusercontent.com/whiteheap/residue-ui/main/docs/assets/hero.png" width="830" alt="Reclaim your storage from Git worktrees, in a Mac app.">
</picture>
</p>

**Every check, size and removal in its window comes from the residue CLI, and nothing moves to the trash until you confirm the plan residue shows.**

```sh
curl -fLO https://github.com/whiteheap/residue-ui/releases/latest/download/residue-macos.dmg
open residue-macos.dmg
```

Then drag residue to Applications. It needs macOS 13 or later, on Apple silicon or Intel, and nothing else: residue is inside. It is not notarized yet, so macOS may block the first launch: [First launch](https://github.com/whiteheap/residue-ui#first-launch) has the steps.

Worktrees sizes each worktree by the space removing it frees, and shows what keeps each one. Restore lists what residue can bring back, and Freed what it has freed.

<p>
<img src="https://raw.githubusercontent.com/whiteheap/residue-ui/main/docs/screenshots/worktrees.png" width="830" alt="The Worktrees screen: a line that says automatic cleanup freed about 70.3 MB, 1 worktree, since the app was last open, with a link to Freed. Below it, 1.3 GB reclaimable, 6 of 11 worktrees can go, about 975 MB freed in the last 7 days. A treemap sizes each worktree by the space removing it frees, grouped by repository: white for can go, gray for kept, hatched for unknown. Below it, each worktree's checks and verdict.">
</p>

<p>
<img src="https://raw.githubusercontent.com/whiteheap/residue-ui/main/docs/screenshots/restore.png" width="830" alt="The Restore screen: 237 MB reclaimable in 2 trash entries, then what residue can bring back, newest first. Each removed worktree's row gives its name and branch, how long ago and by what it was removed, the space that freed, the date it is restorable until at least, its path, and the ignored files it comes back without. The newest, acme-mobile-release-2-5, was removed just now by residue watch because its upstream branch was deleted: 70.3 MB freed, restorable until at least Jan 31, 2027, 12 weeks after its removal, and it comes back without node_modules/ (1 file, 70.3 MB). The rows removed by residue remove are restorable until at least Dec 8, 2026, 30 days after their removal. A trash entry, moved to the trash 2 days ago, holds 132 MB until the first cleanup after 7 days deletes it and leaves a removal record. Each row has a Restore button.">
</p>

<p>
<img src="https://raw.githubusercontent.com/whiteheap/residue-ui/main/docs/screenshots/freed.png" width="830" alt="The Freed screen: 975 MB freed in the last 7 days, 2.1 GB in the last 30, 5.9 GB all time and 215 MB since the app was last open, a column for each of the last 12 weeks, the space each command freed (residue watch, residue remove --all and residue remove by hand), and the space freed in each repository, most first.">
</p>

The screenshots show example repositories and a made-up history of removals.

Source: [github.com/whiteheap/residue-ui](https://github.com/whiteheap/residue-ui)

## The name

Whiteheap joins white hat and heap. A white hat is a hacker who finds weaknesses so they can be fixed, and works in the open. The heap is the memory a program asks for while it runs.
