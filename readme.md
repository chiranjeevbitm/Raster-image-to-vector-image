# Converting the Raster images(jpg ,png,bitmap..etc) to vector images(svg,dxf,...etc) using the potrace tool
	   
DESCRIPTION

	I have used the open source tool call the potrace

	About potrace
		Potrace(TM) is a tool for tracing a bitmap, which means, transforming a bitmap into a smooth, scalable image. The input is a bitmap (PBM, PGM, PPM, or BMP format), and the output is one of several vector file formats. A typical use is to create SVG or PDF files from scanned data, such as company or university logos, handwritten notes, etc. The resulting image is not "jaggy" like a bitmap, but smooth. It can then be rendered at any resolution



# COMPILATION
	just goto the website http://potrace.sourceforge.net/	and download the suitable source code

	If you are installing from sources, just do "make install" as root.
	If you are installing from a binary distribution, just copy the "potrace" and "mkbitmap" binaries to a place where the operating system expects them, such as /usr/local/bin. Also copy the files "potrace.1" and "mkbitmap.1" to a directory where the operating system looks for man pages, such as /usr/local/man/man1.


	
	for windows 

	The distribution includes the executable programs potrace.exe and
	mkbitmap.exe. You need to move these files to a place where Windows looks for programs, for example C:\WINDOWS. Alternatively, you can amend your PATH environment variable, by adding something like the following line to C:\AUTOEXEC.BAT:


Potrace is built from sources using the standard configure/make commands. Please see the file INSTALL for generic installation instructions, and the file README for compile time configuration options specific to Potrace. Some pre-compiled binary distributions are also available. See the file README for instructions on how to install Potrace from a binary distribution. Additional instructions for Windows users are contained in the file README-WIN
All files are in their setup files respectively. 


# Running Commands

	Running the commands for conversion --
	To convert into the bit map format
		because potrace only supports bitmap to vector file

		convert input.jpg output.ppm

		If convert command is not working then download imagemagick library,generally it is preinstalled
		
		https://imagemagick.org/script/download.php

    To convert into the vector file
		potrace -s output.ppm -o svgout.svg



