# Galactic Library Material
This repository houses various materials I create for the [Galactic Library Wiki](https://www.galacticlibrary.net/wiki/Main_Page). This material is mainly exposed for public maintenance of any created material by others working on Galactic Library. 

Since this is material for the Galactic Library, all content in this repository runs under the CC-BY-SA liscence of Galactic Library. 

## Graphics
The graphics hosted here were created using LaTeX TikZ, exported and processed into standalone vector and/or raster images for use on Galactic Library.. Both the LaTeX generating code and various processed end results are preserved here. 

#### Reproducing the graphics 
The original files were created and compiled in Overleaf using pdfLatex. Any similar LaTeX enviroment should compile the files. 

For producing SVG files, the workflow I chose was to compile to normal PDF, then the PDF was imported one page at a time in Inkscape using Poppler/Cairo library. Text was rendered to curves on Import. Export as SVG out of Inkscape. Further editing was done in Affinity Designer in my case.

If you want to edit text outside of LaTeX, you should install expanded font packages of the Computer Modern fonts used by LaTeX. Your import may screw up the fonts otherwise.  

From this point onward, you can repackage the graphics as you want. 

Alternatively, you *could* try pdf2svg and associated packages of LaTeX `standalone` package. I did not experiment with this pipeline due to its indicated fragility. If you manage to find something that works for building good SVGs from these files, please, let me know! 


