# Repo for reproducing a renovate bot bug (or missing feature)

This project has a git submodule to a repo called `renovate-bot-reproduction-recursive-submodules-sub1`.

And this repo has again a submpdule to a repo called `renovate-bot-reproduction-recursive-submodules-sub2`.

So there are two nested submodules recursivly.

You can clone the whole repo tree with `git clone --recursive ..` or update the submodules with `git submodule update --recursive`.

# Current behavior

The renovate bot only clones the repo and pulls the first level of submodules but skips the nested submodule.

# Expected behavior

The renovate bot should clone the repo recursivly with all (nested) submodules.

# Link to the Renovate issue or Discussion

TBA
