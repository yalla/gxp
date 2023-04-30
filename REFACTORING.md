# Rationale

`gxp` is a real useful cluster shell which I really liked back when I was maintaining large-scale systems with thousands of nodes. It's not my job anymore, but lately I needed it again and realized it wouldn't work with 'modern' versions of Python.

Hence my plan is to make it runnable again.

This document tracks the status & efforts.

# Things to do for Python3 refactoring

[x] Replace all instance of the pattern `except select.error,e` with `except select.error as e`
[ ] Replace `cPickle` imports with `import _pickle as cPickle`
[ ] Fix key-lookups in dictionary
[ ] replace all occurences of `string.atoi()` with simple `int()`
[ ] put print statements in paranthesises
