# Wormhole Graphics
These illustrations were created for the article on [wormholes](https://www.galacticlibrary.net/wiki/Wormholes) on Galactic Library. 

The aim here is to cover various geometry situations of wormhole networks. 

One portion of the material is about Wormholes and time travel, aimed at supporting a simple explanation introducing people to the notion of space-time connections, the resulting geometry, and how we may construct Closed Timelike Curves with two example cases. See the subsection of the article for the explanation and context. 

TBA: the other section of the material illustrates properties and consequences of various wormhole networks with various constraints. 

The aim of the illustrations overall is to provide visual images that help people easier understand the problem and behavior space of wormholes and networks of wormholes in space-time. Having visuals to go along with the discussion helps a lot in keeping track of what is happening and why. 

## The TikZ mechanics 
LaTeX TikZ ecosystem is used to generate the graphics programmatically from source code. Ideally, no further editing of the SVG outputs should be required. (in this case, some text was adjusted by moving it.) 

Most introdictionary TikZ graphics are plotted in 2D coordinate space, but TikZ supports 3D coordinate systems and perspective rendering using its [`3d`](https://tikz.dev/library-3d) library. This library also provides different coordinate spaces. 3D cylindrical coordinate space is used since it allows for good programming of the space directions (angle, first length) and time (second length) positions in the space-time diagram. 

A further helpful tool used here to create the perspective is the `tikz-3dplot` [**package**](https://ctan.org/pkg/tikz-3dplot) (it's a package, not a tikz library! Different import statements) which provides useful tools for rotating the drawing frame using `\tdplotsetmaincoords`. 

`calc` provides internal automation to run some `foreach` loops, which generates mainly the background grid. It can be used to repeatedly draw other shapes, however. 

`tikzmarks` is used to create coordinate points for later use. 

`fit,shapes,snakes, arrows` provide further styling options for the connecting arrows. 

`xcolor` provides an expanded means to set, mix and define colors and transparencies. See https://en.wikibooks.org/wiki/LaTeX/Colors
