spacewalk-debian-sync
=====================

An improvised repo-sync to bring Debian packages into Spacewalk

spacewalk-add-debian-multiarch-header.py
========================================

Script to add missing 'Multi-Arch' headers into the Packages files
You need to use this modified version of Steve Meiers spacewalk-debian-sync
script, which will create a temporary file within /tmp with

- `<name> <version> <architecture> <multi-arch>`

for each package with a Multi-Arch header found, while the Packages files
gets parsed.
