du+
=======

du+ - Know file space usage; to hunt the disk hogs

I created my version of du to hunt the disk hogs on a server. 
I planned to prototype it in bash and then write it in haskell.
(The haskell part hasn't happened yet.)

Incidentally this has examples of most of the bash tricks that I ever need; so it works as a reference as well.

Has its own test built in, that creates an example directory tree and then runs du+ againast it.

du+  -test

########
# BUGS #
########
#
# Currently known:
#   * Does not handle dirs that have a space as their first char (not properly escaped or quoted?)
#   * du+ -test|grep C # shows that we have some stray | (not inheriting properly?)
#   * args should work in any order
#
# Feel free to fix them and push them to me on github

# We could add datetime for each file and/or dir (as an option)
# We could accept multiple paths

