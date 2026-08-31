# EP-003 - Linux Files & Directory Operations

**Series:** From Beginner to SOC Analyst

**Phase:** Linux Fundamentals

**Episode:** 003

**Topic:** Linux Files & Directory Operations

**Status:** ✅ Completed

---

## Mission

Investigated how to safely create, copy, rename, move, and remove files and directories without modifying original evidence.

## Commands Learned

- mkdir
- touch
- cp
- mv
- rm
- rmdir

## Key Concepts

- Creating directories
- Creating files
- Copying files
- Moving files
- Renaming files
- Deleting files
- Deleting empty directories
- Evidence preservation

## Biggest Takeaway

Good file management is essential during security investigations. Analysts should preserve original evidence and perform analysis on copies whenever possible.

## SOC Perspective

During incident response, analysts need to organize investigation files while protecting evidence.

A common approach is:

- Preserve the original file.
- Create a copy.
- Analyze the copy.
- Keep investigation folders organized.

## Interview Questions

- What is the difference between `mkdir` and `touch`?
- What is the difference between `cp` and `mv`?
- Why is `rm` considered dangerous?
- What is the purpose of `rmdir`?
- Why should analysts avoid modifying original evidence?

## Things to Remember

- `mkdir` creates directories.
- `touch` creates empty files.
- `cp` copies while preserving the original.
- `mv` moves or renames files.
- `rm` permanently deletes files.
- `rmdir` deletes only empty directories.
- Never analyze original evidence directly.

## Biggest Challenge

Remembering when to use `cp` versus `mv`.

## Next Episode

Viewing and Searching Files

**Commands:**

- cat
- less
- head
- tail
- grep