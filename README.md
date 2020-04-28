otw
===

Tooling and solutions for [OverTheWire](https://overthewire.org) war games.

## Setup

* Clone the repository and `cd` into it.
* Run `export PATH="$PWD/bin:$PATH"`.
* (Optional) Run `rm flags/*` to delete the flags.

## Example Usage (Linux)

* `flag bandit27 | xclip -selection clipboard`: copies the flag for the machine
  `bandit27` to the clipboard.
* `bandit 27`: opens an SSH connection to bandit27@bandit.labs.overthewire.org.
* `echo "deadbeef" > flags/bandit34`: writes the flag `deadbeef` to `bandit34`.
