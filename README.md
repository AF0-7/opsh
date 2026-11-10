# opsh — mini-shell in Python

opsh is a small command-line shell, like a very simple `bash`, written in Python.
You type a command, opsh runs it, shows the result, and waits for the next one.

## About

opsh is a university project built by a team of 4 second-year computer engineering
students. The goal is to understand how a real shell works by building one ourselves:

- reading and splitting what the user types into a command and its arguments
- running programs installed on the system (`ls`, `cat`, `grep`, ...)
- handling **builtins**: commands the shell runs itself, like `cd` and `exit`
- managing files and processes on Linux

We use only Python's standard library, with no external packages.

- **Course:** _to fill in_
- **University:** _to fill in_
- **Year:** 2026–2027

## Team

| Member | Role |
|--------|------|
| _Name 1_ | Team lead |
| _Name 2_ | _to fill in_ |
| _Name 3_ | _to fill in_ |
| _Name 4_ | _to fill in_ |

## Requirements

- Linux (we use WSL Ubuntu on Windows)
- Python 3
- Nothing else to install

## Getting started

```bash
gh repo clone AF0-7/opsh
cd opsh
python3 code/opsh.py
```

Type a command at the opsh prompt. Type `exit` to quit.

## Features

Planned. We tick each one when it works.

- [ ] Run system commands with arguments (`ls -l`, `echo hello`)
- [ ] Builtin commands (see the table below)
- [ ] Aliases (short names for longer commands)
- [ ] Command history, saved in `.opsh_history`
- [ ] Output redirection (`ls > f.txt`, `ls >> f.txt`)
- [ ] Clear error messages for unknown commands

## Builtins and aliases

| Command | Alias | What it does | Status |
|---------|-------|--------------|--------|
| `cd <dir>` | | Change the current directory | planned |
| `pwd` | | Print the current directory | planned |
| `exit` | | Quit opsh | planned |
| `history` | | Show previous commands | planned |
| `alias` | | Create or list aliases | planned |
| `help` | | List the builtins | planned |

## Project structure

```
opsh/
├── code/        source code (opsh.py goes here)
├── tests/       tests
├── README.md    this file
├── .gitignore   files Git must not track
└── .gitattributes  forces Linux line endings (LF)
```

## How we work

1. Get the latest version: `git switch main && git pull`
2. Make a branch for your task: `git switch -c feature/my-task`
3. Commit small steps: `git add <files>` then `git commit -m "What changed"`
4. Push your branch: `git push -u origin feature/my-task`
5. Open a Pull Request on GitHub so a teammate can review it before it goes into `main`
