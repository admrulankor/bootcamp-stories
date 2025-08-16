As a long-time GNU/Linux user, Plan 9's model is more relevant than ever. GNU/Linux as an ecosystem is decidedly gotten worse over time, not better. In fact, that's one of the major reasons I use Plan 9 or one of its derivativesfor my computing.

The Plan 9 philosophy is working smarter instead of harder by leveraging UNIX principles and the synergy it brings along with it. Nothing else comes close to that except BSD, but even that's not really comparable, only that it's a highly engineered product.

With that being said, Plan 9 is not another flavor of GNU/Linux. If you expect it to be, you will have a bad time.

Here's a fraction of the things I think Plan 9 improves on:

* The rc shell fixes a lot of deficiencies in the Bourne shell.
* Per-process namespaces obsolete a whole lot of things like symlinks.
* There is no superuser (root account). This is obsoleted by an auth server called Factotum.
* Uses its own compiler suite that makes cross-compilation particularly easy, compared to the mess of doing so with GCC. 
* Uses its own much cleaner libc routines that are quite distinct from POSIX or the messy glibc additions of today
* Has its own thread library, as well.
* All network information is stored in a text file database mounted on a file server.
* The default file system (Venti) is inherently versioned, introspectable and has backup built into it. You can do things like swap in libraries from cache and revert changes without a hitch.
* Everything is statically linked.
* Uses mk instead of make.
* A lot of things like recursive copy and find aren't built into the standard commands. It's expected you actually chain together commands instead of reinventing the wheel for every single operation. The canonical example is the use of du to walk the file system tree, for everything. This replaces find and other things.
* Designed not just to be multi-user, but multi-tenant. Makes many uses for containers and access controls unneeded because of its core design.

Try it. It's more relevant now than ever.