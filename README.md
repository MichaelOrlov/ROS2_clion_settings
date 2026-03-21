# Introduction

This repository provides CLion style settings which are as close as possible to ROS 2 coding style
found here: https://github.com/ros2/ros2/wiki/Developer-Guide#language-versions-and-code-format

# Usage

In CLion go to *File - Settings Repository* and add this repository as *Upstream URL*.
Afterward click *Merge* or *Overwrite Local*.

# Fix for missing local changes tab in Git panel

## Problem

After updating the IDE to the 2025.1+ release from an earlier version, the "Local Changes" tab in
the "Git" tool window is missing.

## Cause

The "Local Changes" tab and modal commit dialog were moved under a separate plugin, and option to
activate them were also moved within the IDE settings. More information about the decision and
discussions about the results can be found here:
https://youtrack.jetbrains.com/projects/IJPL/issues/IJPL-177161.

## Resolution

To enable the "**Local Changes**" tab and modal commit interface:
1. Install and enable the Modal Commit Interface plugin in Settings (⌘ + , or Ctrl + Alt + S) >
   Plugins.
2. Enable the option Settings (⌘ + , or Ctrl + Alt + S) > Advanced Settings >
   Version Control > Use modal commit interface for Git and Mercurial
3. Disable the option Settings (⌘ + , or Ctrl + Alt + S) > Version Control > Git > Enable staging 
   area

Reference to original article
https://youtrack.jetbrains.com/articles/SUPPORT-A-1996/Local-Changes-Tab-Missing-after-IDE-update-to-2025.1