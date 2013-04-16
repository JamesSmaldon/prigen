prigen
======

A small script for generating a Qt QMake .pri project include file from a
Visual Studio 2010 project.

prigen is useful for cross platform C++ projects written primarily in Visual
Studio with the Qt framework, where Qt creator is also used as a secondary IDE
for development of the project on unix-like operating systems. The Qt assistant
for Visual Studio provides a feature for generation of pri include files for a
selected project, but the process cannot be automated as part of the build.
This means that every time source files are added or removed from a project,
the .pri files must be manually regenerated. Prigen can be executed in a
post-build script to automatically generate the .pri files.

Requirements:
Python 2.7

Usage:
python prigen.py \<input vcxproj.filters filename\> \<output pri filename\>

Tested with Visual Studio 2010 and Qt 4.7.4.
