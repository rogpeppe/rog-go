Some Go packages that some people may find useful.

### canvas ###

An experimental package for drawing and manipulating graphical widgets.
Based on exp/draw, exp/draw/x11 and freetype-go.googlecode.com/freetype/raster.
Still in its very early stages.

Install with: `goinstall rog-go.googlecode.com/hg/canvas`

### values ###
Multiple-reader, multiple-writer, typed values. Designed for
notification in a GUI environment.
Install with: `goinstall rog-go.googlecode.com/hg/values`

### cmd/bounce ###

A command that bounces balls inside a window.
Each ball represents a single goroutine.
Use button 1 to draw lines for the balls to bounce off,
button 2 to create new balls, and button 3 to delete a ball.
There's a slider at the top level that allows the update
interval to be changed.

Build with:
```
    goinstall rog-go.googlecode.com/hg/x11
    cd $GOROOT/src/pkg/rog-go.googlecode.com/hg/cmd/bounce
    make
```

### cmd/hello ###

A simple(ish) program to display some text and
allow the user to drag it around.

Build with:
```
    goinstall rog-go.googlecode.com/hg/x11
    cd $GOROOT/src/pkg/rog-go.googlecode.com/hg/cmd/hello
    make
```

### cmd/shape ###

Play with the freetype rasterization code.
Click with button 1 to start a new shape;
further button clicks add more points to the
shape. Button 2 makes the new point part of
a curve (once for quadratic, twice for cubic).
Button 3 ends the curve. Once a curve has been
completed, the points on the curve may be
dragged to change the shape.

Build with:
```
    goinstall rog-go.googlecode.com/hg/x11
    cd $GOROOT/src/pkg/rog-go.googlecode.com/hg/cmd/shape
    make
```