# git-p4
Copied from the git official repo with some specific fixes. Put this in your
`$PATH` so you can override the default `git p4` commands.

# git-p4-shelve
A utility to automatically create or update P4 shelves from git commits. See
`git-p4-shelve --help` for more info.

# git-autosquash
A utility to squash all commits in 'branch' to 'squashed/branch'. Useful for
preserving git history before shelving to P4, e.g.:

If on branch `my-feature`, squash to `squashed/my-feature`:

    git-autosquash p4/master

Shelve the new branch in P4:

    git-p4-shelve -U squashed/my-feature

(You can also do this with `git-p4-shelve --squash`.)
