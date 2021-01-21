YaST - The Pattern Definitions
==============================

[![Workflow Status](https://github.com/yast/yast-patterns/workflows/CI/badge.svg?branch=master)](
https://github.com/yast/yast-patterns/actions?query=branch%3Amaster)

This meta package defines the YaST software patters which can be installed using
the package manager.


Getting the Sources
===================

To get the source code, clone the GitHub repository:

    git clone https://github.com/yast/patterns-yast.git

If you want to contribute into the project you can
[fork](https://help.github.com/articles/fork-a-repo/) the repository and clone your fork.


Contact
=======

If you have any question, feel free to ask at the [development mailing
list](http://lists.opensuse.org/yast-devel/) or at the
[#yast](https://webchat.freenode.net/?channels=%23yast) IRC channel on freenode.


Notes
=====

### Maintenance

- This repository contains the YaST patterns for the SLE15/Leap 15.0 (and newer) products,
  see the respective Git branches.
- The patterns for the older products are defined in the internal OBS together with
  the other SLE patterns. For example:
  - The [SLE12-SP5 SDK-YaST](
      https://build.suse.de/package/view_file/SUSE:SLE-12-SP5:GA/patterns-sdk/patterns-sdk.spec?expand=1
    ) pattern
  - The [SLE12-SP5 yast2](
      https://build.suse.de/package/view_file/SUSE:SLE-12-SP5:GA/patterns-sles/patterns-sles.spec?expand=1
    ) pattern
