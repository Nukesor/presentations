---
theme:
  override:
    code:
      alignment: left
      background: false
---

presenterm
===

https://github.com/mfontanini/presenterm

- Präsentations tool
- Auf der Commandline
- Geschrieben mit Markdown

![](doge.png)


<!-- end_slide -->
presenterm - code highlighting
===


```rust +line_numbers
#[derive(Clone, Debug)]
struct Person {
    name: String,
}
```
<!-- pause -->

* **Bold text**.
* _Italics_.
* **_Bold and italic_**.
* ~Strikethrough~.

<!-- pause -->

| Name   | Taste  |
| ------ | ------ |
| Potato | Great  |
| Carrot | Yuck   |


<!-- end_slide -->
upterm
===

https://github.com/owenthereal/upterm

- Modern `tmate` alternative
<!-- pause -->
- **Without** `tmux`
<!-- pause -->
- Written in Go
<!-- pause -->
- `upterm host --read-only`


<!-- end_slide -->
atuin
===

https://github.com/atuinsh/atuin

- Shell history searcher
<!-- pause -->
- Fuzzy search
<!-- pause -->
- Great configurability
<!-- pause -->
- With local sqlite database


<!-- end_slide -->
Custom Filters
===

- History filters to simply hide uninteresting commands that clutter your history.

```toml
history_filter = [
  # Day-to-day shell commands
  "^cd .*",
  "^cd$",
  "^fg",
  "^ls",
  "^git diff .*",
]
```

- Possible to only add "successful" commands to history.


<!-- end_slide -->
Server (optional)
===

- Synchronization across devices!
<!-- pause -->
- Can use public server (client side encrypted)
<!-- pause -->
- Selfhosting is super easy (single-binary + database)


<!-- end_slide -->
zoxide
===

https://github.com/ajeetdsouza/zoxide

- Smart cd command
<!-- pause -->
- Integrates itself into shell session
<!-- pause -->
- Jump to common folders directly
<!-- pause -->
- No longer do `cd ../repos/web/my_project/backend`
- Instead do `j back` from anywhere


<!-- end_slide -->
bat
===

https://github.com/sharkdp/bat

- Modern `cat`/`tail`/`head` pager alternative.
<!-- pause -->
- It's just nice
  - Syntax highlighting
  - Line numbers


<!-- end_slide -->
btop
===

https://github.com/aristocratos/btop

- Beautiful configurable `ctop` & `htop` alternative
- Good visual shortcuts.


<!-- end_slide -->
ripgrep
===

https://github.com/BurntSushi/ripgrep

- Modern `grep` alternative
<!-- pause -->
- Sane defaults
```sh
grep -r --include='*.rs' --exclude-dir='target' 'struct' .
rg --glob  '*.rs' struct
```
<!-- pause -->
- Respects .gitignore
<!-- pause -->
- Beautiful
<!-- pause -->
- Freaking fast


<!-- end_slide -->
fd
===

https://github.com/sharkdp/fd

- Modern `find` alternative
<!-- pause -->
- Sane defaults
```sh
find . -path ./target -prune -o -name "*.rs" -print
fd \.rs
```
<!-- pause -->
  - Respects .gitignore
<!-- pause -->
- Beautiful
<!-- pause -->
- Freaking fast


<!-- end_slide -->
git-delta
===

https://github.com/dandavison/delta

- Beautiful git diffs
- Relatively straight forward to integrate into git
- Good visualization
  - Syntax highlighting
  - Line numbering
  - Side-by-side or stacked view possible


<!-- end_slide -->
bandwhich
===

https://github.com/imsnif/bandwhich

- CLI bandwidth monitoring tool
- Good to get a good first impression


<!-- end_slide -->
dust
===

https://github.com/bootandy/dust

- Modern `du`
- Sane defaults
- Nice tree view with heuristics on what to show
  - Large folders/files are prioritized


<!-- end_slide -->
skim
===

https://github.com/junegunn/fzf
https://github.com/skim-rs/skim

- Commandline fuzzy finder
- Useful to create custom selector/fuzzy finding CLI "widgets".


<!-- end_slide -->
yazi
===

https://github.com/sxyazi/yazi

- Quite clean and modern CLI file manager

<!-- end_slide -->
