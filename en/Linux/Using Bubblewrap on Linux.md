---
title: 
aliases: 
tags:
  - English
draft: false
status: Backlog
---
> [!todo]

Bubblewrap is a sandboxing tool on Linux that creates isolated environments for applications, enhancing security and reducing potential conflicts between software.
^desc
It's utilized by Flatpak to isolate apps launched from software packages. The command-line interface for Bubblewrap is `bwrap`, and it allows users to construct a root filesystem and process environment within a new, empty mount namespace. This namespace is on a tmpfs that is invisible from the host and is automatically cleaned up after use. Bubblewrap is particularly useful for running applications with a reduced risk of system interference or vulnerability exploitation.
# Sources
- 