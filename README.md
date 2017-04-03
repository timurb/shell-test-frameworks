Shell test frameworks
=====================

This is a list of test frameworks and related tools in pure shell.

Sort order is random.

Last commits for the frameworks are noted by 2017-04-03.

#### [Roundup](http://github.com/bmizerany/roundup)

Last commit: [Jan 27, 2015](https://github.com/bmizerany/roundup/commits/master)

Features:
* test autorunner
* test case fails and aborts on first non-zero exit code
* setup/teardown
* skipping tests

Test cases:
* coded in spearate functions with naming like `it_.*()` (RSpec-like)
* are searched in files passed as commandline parameters or in a current file with special shebang

Output: custom human-readable format.

Installer: configure-make-based installer provided.

Codebase consists of a single file.

#### [BATS](http://github.com/sstephenson/bats)

Last commit: [Feb 19, 2016](https://github.com/sstephenson/bats/commits/master)

Features:
* test autorunner
* test case fails and aborts on first non-zero exit code
* setup/teardown
* helper functions to ease doing several asserts per test case
* no tests skipping (probably can be done by modifying function names)

Test cases:
* coded in spearate functions with naming like `@test ".*"()`
* are searched in files passed as commandline parameters or in a current file with special shebang

Output: [TAP](http://en.wikipedia.org/wiki/Test_Anything_Protocol) format.

Installer: install.sh provided to do installation
Codebase consists of several files

#### [Sharness](https://github.com/chriscool/sharness)

Last commit: [Sep 9, 2016](https://github.com/chriscool/sharness/commits/master)

* assertions are eval-ed

#### [Shpec](https://github.com/shpec/shpec)

Last commit: [Apr 2, 2017](https://github.com/rylnd/shpec/commits/master)

Features:
* test autorunner (RSpec-like): accepts parameter with tests
* describe/it blocks
* various assert functions
* custom matchers supported
* assertions are eval-ed
* stubbing commands
* failing assertion continues evaluation
* no setup/teardown functions
* color output

Test cases:
* run in the same process

Outuput: [RSpec](http://en.wikipedia.org/wiki/RSpec)-like format.

Installer: installation not needed but can be done via install.sh or a makefile

Codebase is very small and clear although looks not to be very portable.

#### [Shunit](http://shunit.sourceforge.net/)

Last commit: 2 Nov 2008


#### [Shunit2](https://github.com/kward/shunit2)

Last commit: [Mar 16, 2017](https://github.com/kward/shunit2/commits/master)

Features:
* test autorunner
* various assertXXX functions
* failing assertion produces message but does not abort test case
* setup/teardown
* failing/skipping tests

Test cases:
* coded in spearate functions with naming like `test.*()`
* are searched in currently loaded plain shell script

Wide range of shells and OSes is supported.

This can also be obtained by `apt-get install shunit2` in Ubuntu or searched for various forks/clones on github.

Output: custom human-readable format.
Codebase consists of a single file.

---
See also [shflags](http://code.google.com/p/shflags/) and [log4sh](https://sites.google.com/a/forestent.com/projects/log4sh)
of the same author which are commandline param processing library and logging library respectively.

#### [kal-shlib-shunit](https://github.com/vaab/kal-shlib-shunit)

Last commit: [Apr 30, 2012](https://github.com/vaab/kal-shlib-shunit/commits/master)

(3 commits in total for the whole lifetime)

#### [shell-unittest](http://git.altlinux.org/gears/l/libshell.git?p=libshell.git;a=summary) of ALTLinux's libshell

Last commit: [18 Nov 2016](http://git.altlinux.org/gears/l/libshell.git?p=libshell.git;a=log)

Test autorunner searches for test cases in a file pointed to by specific function invocation.

Has very poor documentation.
A part of libshell and not usable without the rest of the library.

Features:
* test autorunner
* various assertXXX functions
* setup/teardown

Test cases:
* coded in spearate functions with special comment placed after function name: `# UnitTest`
* are searched by a special function invocation from a separate file

Output: custom human-readable format.
Codebase for the whole library consists of several files.

Installer: make-based installer provided.

#### [tapper-autoreport](https://github.com/tapper/Tapper-autoreport) 

Last commit: [22 Sep 2014](https://github.com/tapper/Tapper-autoreport/commits/master)

Not an actually testing framework but a library to easily produce output from your script in [TAP](http://en.wikipedia.org/wiki/Test_Anything_Protocol) format.

It seems to carry much legacy stuff in it and I could not actually run it (although I didn't try very hard with it).

Output: [TAP](http://en.wikipedia.org/wiki/Test_Anything_Protocol) format.

#### [testlib.sh](https://gist.github.com/3877539)

Last commit: [13 Feb 2013](https://gist.github.com/rtomayko/3877539/revisions)

#### [ts](https://github.com/thinkerbot/ts)

Last commit: [Jun 1, 2016](https://github.com/thinkerbot/ts/commits/master)

#### [wvtest](https://github.com/apenwarr/wvtest)

Last commit: [Jun 9, 2015](https://github.com/apenwarr/wvtest/commits/master)

Not an actually testing framework but a library to easily produce output in custom test-result format.
