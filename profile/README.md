Open-source tools and infrastructure for agents, developers and security teams, all in Rust.

Agents now write code, run commands and hold credentials on real machines, but most of the tools around them were built for one person at a keyboard. Whiteheap builds tools for that shift.

We want absolute excellence in software. Each tool leaves your work alone whenever it cannot tell what is safe to touch, and says what it did in a few words. It uses as little CPU and memory as it can, and we measure both on each code change before it ships. Each tool is one Rust binary with as few dependencies as we can manage, and every release carries SHA-256 checksums and a build-provenance attestation.

## Tools

### [residue](https://github.com/whiteheap/residue)

Reclaim your storage from Git worktrees, automatically and safely. residue removes a worktree only when nothing in it would be lost, whichever coding agent left it. It runs on macOS, Linux and FreeBSD, and comes with a Mac app.

The install script installs residue and, on macOS and Linux, turns on automatic cleanup:

```sh
curl -fsSL https://residue.whiteheap.com/install.sh | sh
```

Homebrew alone installs residue without automatic cleanup: `brew install whiteheap/tap/residue`. Website: [residue.whiteheap.com](https://residue.whiteheap.com)

## The name

Whiteheap joins white hat and heap. A white hat is a hacker who finds weaknesses so they can be fixed, and works in the open. The heap is the memory a program asks for while it runs.
