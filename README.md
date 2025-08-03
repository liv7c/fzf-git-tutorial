# fzf with Git and Bash Tutorial

Learn to build Git helpers with fzf and Bash from scratch.

This repository contains the code examples from the blog post: [**Build Git helpers from scratch with Bash and fzf**](https://oliviac.dev/blog/build-git-helpers-bash-fzf).

## What you'll learn

- How to combine `fzf` with Git commands
- Writing Bash functions (with some scripting tips)
- Building interactive branch switchers
- Creating safe deletion helpers with confirmation
- Making a commit selection tool for rebasing

## Quick start

1. **Install fzf**: check out the [installation instructions for fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation).


2. **Clone this repository**:

   ```bash
   git clone https://github.com/yourusername/fzf-git-tutorial.git
   cd fzf-git-tutorial
   ```

3. **Source the helpers**

   Add this to your `~/.bashrc` (or `~/.bash_profile`):

   ```bash
    # in your ~/.bashrc
    source /path/to/fzf-git-tutorial/.bash_helpers
   ```

   Then reload your shell:

   ```bash
   source ~/.bashrc
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

This repository is designed for learning and exploring Bash scripting with `fzf`. For a more robust and feature-rich solution, check out [fzf-git.sh](https://github.com/junegunn/fzf-git.sh).

## Requirements

- Bash (tested with 5.2+)
- fzf (tested with 0.65+)
- Git

## Blog post

Read the full tutorial: ["Build Git helpers from scratch with Bash and fzf"](https://oliviac.dev/blog/build-git-helpers-bash-fzf). 

## License

MIT
