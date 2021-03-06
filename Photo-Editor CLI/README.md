# Photo Editor

Chelcea Claudiu Marian

Contact at: claudiuchelcea01@gmail.com

I created a photo editor for the faculty homework that receives text commands and supports performing a set of operations over PPM (portable pixmap format) -RGB- and PGM (portable graymap format) -GRAYSCALE- image file formats, both as plain (ASCII) text or binary files.

|        TYPE        |        ASCII        |        BINARY       |               COLORS                |
| ------------------ | ------------------- | ------------------- | ----------------------------------- |
|      GRAYSCALE     |         P2          |         P5          |    0 - 255 (black & white shade)    |
|      RGB           |         P3          |         P6          |            16.777.216 (RGB)         |


# RUN EXAMPLE: 
"I:" represents keyboard typed command <br>
"O:" represents the output message<br><br>
I:LOAD test_file  <br/>
O;Loaded test_file <br/>
I:SELECT 0 1 8 10 <br/>
O;Selected 0 1 8 10 <br/>
I:CROP<br/>
O;Image cropped<br/>
I:SAVE my_binary_file<br/>
O;Saved my_binary_file<br/>
I:LOAD non_existent_file<br/>
O;Failed to load non_existent_file<br/>
I:LOAD color_file<br/>
O;Loaded color_file<br/>
I:GRAYSCALE<br/>
O;Grayscale filter applied<br/>
I:SEPIA<br/>
O;Sepia filter not available<br/>
I:SAVE my_plain_file ascii<br/>
O;Saved my_plain_file<br/>
I:EXIT<br/>

# GENERATE YOUR OWN IMAGE:
To generate your own PNM and PGM files, use the "convert" utility that converts png / jpeg / jpg files to these formats:<br/>
• Setup: <br>
$ sudo apt update <br>
$ sudo apt-get install build-essential <br>
$ sudo apt-get install imagemagick<br/> <br>
• Documentation: man convert<br/>
• Examples:<br/>
    convert foo.jpg foo.ppm (transforms foo.jpg în foo.ppm, binary RGB)<br/>
    convert foo.jpg foo.pgm (transforms foo.jpg în foo.pgm, binary grayscale)<br/>
    convert foo.jpg -compress None foo.ppm (transforms foo.jpg în foo.ppm, ASCII RGB)<br/>
    convert foo.jpg -compress None foo.pgm transforms foo.jpg în foo.ppm, ASCII grayscale)<br/>
