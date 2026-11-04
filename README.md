<p align="center">
  <b>Jefferson Cesar Antunes</b><br>
  Systems developer — Linux/OpenBSD process introspection and memory analysis
</p>

---

### About

I'm self-taught. Most of what I know comes from reading man pages, breaking
things in VMs, and tracing syscalls until the behavior made sense.

I write small C and Bash tools that I can read end to end. My interest is the
boundary where abstractions stop helping: process state, memory layout, and
what the kernel will and won't tell you.

### Projects

| Project | What it does | Language |
| :--- | :--- | :--- |
| [**PMV**](https://github.com/jeffersoncesarantunes/PMV) | OpenBSD process mitigation viewer. Reads `kinfo_proc` through `kvm(3)` and reports whether `pledge(2)`, `unveil(2)`, and W^X are active per process. It reports presence, not policy depth — the kernel exposes nothing more. | C11 |
| [**K-Scanner**](https://github.com/jeffersoncesarantunes/K-Scanner) | Linux RWX memory scanner. Parses `/proc/[PID]/maps`, flags writable+executable regions, and separates JIT mappings from suspicious ones. | C99 |

Both build with `make`. I'm adding a `make verify` target, behavioral tests,
and a benchmark to each repo.

### Environment

C (C99/C11), Bash, Python · OpenBSD, Arch Linux · Neovim

### Contact

<p align="center">
  <a href="https://matrix.to/#/@striderhiryu:matrix.org"><img src="https://img.shields.io/badge/Matrix-006B4D?style=flat-square&logo=matrix&logoColor=white" /></a>
  <a href="https://x.com/j3ff3rsonc3sar"><img src="https://img.shields.io/badge/X-202327?style=flat-square&logo=x&logoColor=white" /></a>
  <a href="https://codeberg.org/jeffersoncesarantunes"><img src="https://img.shields.io/badge/Codeberg-2185D0?style=flat-square&logo=codeberg&logoColor=white" /></a>
  <a href="https://discord.com/users/1476405883733807247"><img src="https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=discord&logoColor=white" /></a>
  <a href="https://mastodon.social/@jeffersoncesar"><img src="https://img.shields.io/badge/Mastodon-6364FF?style=flat-square&logo=mastodon&logoColor=white" /></a>
</p>

### Issues

If a tool here overclaims or fails on your machine, open an issue with the
command, your OS/kernel version, and the output. That's more useful to me than
a feature request.
