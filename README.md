My git-aliae are snippets of git-related nutcaseness that I use enough to write-down. I've
published them here because I find I often want to refer people to them when I'm asked to
help with git-related issues.

I've officially published those in `/bin`, with a blog post and even some documentation if
you open the command in an editor; but I've also put all my other aliases in `/wip`
(work-in-progress).

As usual with this kind of stuff, there's no guarantee that they do what you want.

Installation
------------

To install the git-aliae, just clone the repository to a known location  (`git clone
git@github.com:ConradIrwin/git-aliae`) and then add `export
PATH=$PATH:/path/to/git-aliae/bin` to your `~/.bashrc`.

If you also want to use the `wip` commands, then `export
PATH=$PATH:/path/to/git-aliae/wip` in addition to the previous line.

Also feel free to just copy and paste commands into any directory that's already in your
`$PATH`.

Command list
------------

Introduced in [Git aliae to make you more awesome](https://cirw.in/blog/git-aliae-1)
* [git amend](https://github.com/ConradIrwin/git-aliae/blob/master/bin/git-amend) — adds more
  stuff to the most recent commit.
* [git uncommit](https://github.com/ConradIrwin/git-aliae/blob/master/bin/git-uncommit) — removes
  stuff from the most recent commit.
* [git pause](https://github.com/ConradIrwin/git-aliae/blob/master/bin/git-pause) — creates a
  temporary commit on the current branch so you can context-switch.
* [git resume](https://github.com/ConradIrwin/git-aliae/blob/master/bin/git-resume) — dissolves
  the commits created by git pause so you can resume work.

Introduced in [Git aliae so that you never lose work](https://cirw.in/blog/git-aliae-2)
* [git cof](https://github.com/ConradIrwin/git-aliae/blob/master/bin/git-cof) — wraps `git
  checkout -f`, but saves your work first.
* [git foc](https://github.com/ConradIrwin/git-aliae/blob/master/bin/git-foc) — undoes the
  most recent `git cof`

FAQ
---

* Surely *aliae* isn't really the plural of *alias*?

Of course not, that would be *aliases*. *aliae* is the feminine plural of the Latin work
*alius* meaning other. Thus, these are just "many other git commands". (They don't
actually use git's alias system, but they work in pretty much the same way).

By the way, the etymology of alias is actually pretty interesting, thanks for asking: It
originally just meant "others" (feminine plural accusative), and came to mean "in another
place, or at another time" in post-Augustan Latin. The English lawyers pounced on this so
that they could say "John Smith, who was 'in another place/at another time' known as
Esther" much more succinctly: "John Smith, alias Esther, ...". This then found its way
into general usage as a noun.

* Why doesn't `--help` work?

Git uses the `man` command to show help, and I haven't gotten around to writing man pages
for these commands yet. Please do send pull-requests if you do :).


Meta-fu
-------

Everything is licensed under the MIT license. Bug reports and pull requests are welcome.
