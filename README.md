# fzf with Git and Bash Tutorial

Learn to build Git helpers with fzf and Bash from scratch.

This repository contains the code examples from the blog post ["The joy of fzf: building Git helpers with Bash"](https://oliviac.dev/blog/fzf-bash-git-helpers).

## What you'll learn

- How to combine fzf with Git commands
- Writing Bash functions along with some Bash scripting tips
- Building interactive branch switchers
- Creating safe deletion helpers with confirmations
- Making commit selection tools for rebasing

## Quick start

1. **Install fzf**: check out the [installation instructions for fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation).


2. **Clone this repository**:

   ```bash
   git clone https://github.com/yourusername/fzf-git-tutorial.git
   cd fzf-git-tutorial
   ```

3. **Install the helpers**. Source this file in your `.bashrc`:

   ```bash
    # in your ~/.bashrc
    source PATH_TO_THIS_REPO/fzf-git-tutorial/.bash_helpers
   ```

4. **Try the helpers** (in any Git repository):

   ```bash
   sfb    # Switch to a branch using fzf
   dfb    # Delete a branch with confirmation
   gri    # Interactive rebase commit selection
   ```

## What's included

- `.bash_helpers` - All the Git helper functions

## The helpers

### `sfb` (Switch Find Branch)

Interactive branch switcher using fzf. Shows all local branches with tracking info and switches to your selection.

### `dfb` (Delete Find Branch)  

Safe branch deletion with fzf selection and confirmation prompt.

### `gri` (Git Rebase Interactive)

Choose a commit to rebase onto using fzf with colored Git log output.

## Educational focus

This repository is designed for learning and making Bash scripting less of a black box. For a more robust and feature-complete solution, check out [fzf-git.sh](https://github.com/junegunn/fzf-git.sh) by the creator of fzf.

## Requirements

- Bash (tested with 5.2+)
- fzf (tested with 0.65+)
- Git

## Blog post

Read the full tutorial: [The joy of fzf: building Git helpers with Bash](https://oliviac.dev/blog/fzf-bash-git-helpers)

## License

MIT
