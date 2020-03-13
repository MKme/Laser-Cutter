# BoxMaker

(Note: This Github Repository is unofficial. It should be considered a fork of the original 
BoxMaker at http://www.keppel.demon.co.uk/111000/111000.html)

A free tool for creating boxes using tabbed construction

version 0.85 - February 27 2012 

please report bugs, comments etc to bugs@twot.eu

# About

This tool is designed to simplify and speed up process of making practical boxes using
a laser cutter (though it can be used with any CNC cutter)  to prepare the pieces.

The tool works by generating a drawing of the pieces of the box with the tab and hole
size corrected to account for the kerf (width of cut), these pieces are composed of sides,
each side being a discreet object, to move a piece in the drawing the edges need to be
grouped together.

# Release Notes

So far no serious bugs( i.e causing runtime errors ) have been found.
The program works with python versions 2.6.5, 2.6.7 and 2.7.2, other version have not yet 
been tried except python 2.5.1 which fails with a syntax error.

This version has been tried on windows XP, windows 7, Ubuntu and Mac OS X with no 
serious problems (the live preview works most of the time but can be flaky).

Only crude input checking has been implemented in the program but as the only output 
is a drawing the worst that can happen is a messed up picture 
(control-Z cures that problem).

# To Do
 
Improve program documentation. Improve input checking to restrict values to correct 
solutions.

# Use

The interface is pretty self explanatory, the extension is 'Tabbed Box Maker' in the 
'Laser Tools' group (hopefully more tools will soon(ish) join it).

In order of appearance:

### Unit
unit of measurement used for drawing

### Box Dimensions: Inside/Outside
whether the box dimensions are internal or external

### Length; Width; Height
the box dimensions

### Minimum/Preferred Tab Width
the size of the tabs used to hold the pieces together

### Tab Width: Fixed/Proportional
for fixed the tab width is the value given in the Tab
Width, for proportional the side of a piece is divided 
equally into tabs and 'spaces' with the tabs size 
greater or equal to the Tab Width setting

### Material Thickness
as it says
 
### Kerf
this is the width of the cut (e.g for 3mm acrylic on an epilog cutter this is
approximately 0.25mm)

### Clearance
this value is subtracted from the kerf in cases where you deliberately want
slightly slacker joints (usually zero)

### Layout/Style
(This is where additions/changes will most likely occur, also having a
problem with live preview: it is best to turn preview off when changing this 
setting)
this setting determines both the type of drawing produced and the way tabs
are used on the sides of pieces.

### Space Between Parts
how far apart the pieces are in the drawing produced

# Installation
 
 Boxmaker.inx and Boxmaker.py need to be put in the inkscape extensions folder
 generally in: 
   ...\Inkscape\share\extensions 
 or linux: 
   usr/.../Inkscape/share/extensions
   (NOTE: you need to make boxmaker.py executable)

# Versions

     0.5    ( 9 oct 2011)   beta
     0.7    (24 oct 2011)   first release
     0.8    (26 oct 2011)   basic input checking implemented
