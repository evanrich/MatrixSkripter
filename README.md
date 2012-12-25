MatrixSkripter
==============
![Sample screen](https://github.com/canosso/MatrixSkripter/blob/master/matrixskripter.png)

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Key features:<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Import
bitmaps with up to 16 <span class=SpellE>colors</span>, match these <span
class=SpellE>colors</span> to the existing 4 <span class=SpellE>colors</span>,
manipulate the bitmap and show this bitmap on the matrix<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Use all
possible <span class=SpellE>colors</span>, from 0 to <span class=GramE>9,</span>
for each pixel is one digit, the <span class=SpellE>color</span> information is
stored in strings for faster communication<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Use any
text as bitmap with any font with any attribute for the matrix<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Use for text
in any language char instead of only <span class=SpellE><span class=GramE>Ascii</span></span>
0-128 chars<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Use all
possible functions of the <span class=SpellE>Lonewolf</span> ht1632c library, </span><a
href="http://code.google.com/p/ht1632c/"><span lang=EN-GB style='mso-ansi-language:
EN-GB'>http://code.google.com/p/ht1632c/</span></a><span lang=EN-GB
style='mso-ansi-language:EN-GB'><o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Test all
data before you save it to the script. You can let run the script in background
over USB or better Ethernet, but it consummates a lot of CPU Power.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Script your
matrix functions and paste an Arduino sketch into the Arduino IDE<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Faster
bitmap drawing, because first the whole matrix will be plotted and then Send
matrix will be sent. Also only the visible pixel will be plotted.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>What is needed?<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>An Arduino
board with serial communication, best over USB, I didn't get the Mega 2560
board to run<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>A Sure
Electronics 32x16 <span class=SpellE>bicolor</span> LED matrix with <span
class=SpellE>Holtek</span> ht1632c chip<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>An Ethernet
shield could be also used for faster testing<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>The SD card
could be used for storing commands, to run the matrix remotely but without
bitmap scrolling<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Why such a mess?<o:p></o:p></span></h1>

<p class=MsoNormal><span class=GramE><span lang=EN-GB style='mso-ansi-language:
EN-GB'>Because the Arduino has no bitmap handling, no <span class=SpellE>color</span>
matching, not so easy possibilities to change the code and limited data
storage.</span></span><span lang=EN-GB style='mso-ansi-language:EN-GB'> <span
class=GramE>That you have to upload the code, if you want to test your content
e.g. where to put the bitmap, is also annoying and takes a lot of time.</span><o:p></o:p></span></p>

<p class=MsoNormal><span class=GramE><span lang=EN-GB style='mso-ansi-language:
EN-GB'>Because the PC can't directly address a LED matrix and can't run
remotely on a simply 9V battery.</span></span><span lang=EN-GB
style='mso-ansi-language:EN-GB'><o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Therefore
you get a tool which use all the bitmap possibilities of a PC, script handling
with no limits except the Arduino data storage limit, almost live testing
(bitmap scrolling is lame over USB) and all 4 <span class=SpellE>colors</span>
at the same time.<o:p></o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Getting started<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Start the
Matrix <span class=SpellE>Skripter</span> and the Arduino <span class=GramE>IDE,</span>
connect your Arduino over USB.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Change the
settings according to your board, especially the number of X-matrix.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Then for
testing select at the menu &quot;Copy Serial Test File to Clipboard&quot; and
copy the test file into the Arduino IDE and upload it.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>If you
uploaded the test file, select your COM port at <span class=GramE>&quot; Select</span>
the Test Matrix Communication method&quot;. The board is now connected with
Matrix <span class=SpellE><span class=GramE>Skripter</span></span><span
class=GramE>,</span> you can test now all functions.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>How to use Matrix <span
class=SpellE>Skripter</span><o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>The
programme looks quite overload but you don't need to know all functions before
you use it.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>All similar
buttons/options have the same <span class=SpellE>color</span> and the same
position on the different tabs:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Beige – Saving
of a text file, those are tab separated and only for the Matrix <span
class=SpellE>Skripter</span> useful<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Green –
Import either a text file or bitmap for the Matrix <span class=SpellE>Skripter</span>
also the font select is green <o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Red – Test
functions or script with the Arduino board connected<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Yellow –
Add data to the Matrix Script<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Blue –
Co-ordinates and delay of a function<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>White – Select
the behaviour of the function<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Grey –
Manipulate the Matrix Script<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>General options<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Each
function has a <span class=SpellE>color</span> field and the option &quot;Send
Frame&quot;, the later could be used either to plot each Line/Text, show the
content on the matrix after it was plotted in background or put the content
only in the memory and the next function will send the content to the matrix.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>At the
white field, you can decided if you want only to show Bitmap/Text or scroll it,
you can also choose the scrolling direction (LEFT | UP and RIGHT | DOWN are
different options) and if you want to scroll blinking (this function is taken
from <span class=SpellE>Lonewolf</span>, shame on me).<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>For
&quot;Input Bitmap&quot; and &quot;Text as Bitmap&quot; there are also rotation
and flip, so you don't need to manipulate the bitmap before import.<o:p></o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Bitmaps and Import Bitmaps<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Bitmaps are
similar to PGM, </span><a
href="http://en.wikipedia.org/wiki/Portable_graymap#PGM_example"><span
lang=EN-GB style='mso-ansi-language:EN-GB'>http://en.wikipedia.org/wiki/Portable_graymap#PGM_example</span></a><span
class=GramE><span lang=EN-GB style='mso-ansi-language:EN-GB'>,</span></span><span
lang=EN-GB style='mso-ansi-language:EN-GB'> they are for each pixel one <span
class=SpellE>color</span>. <o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>For the
matrix you need bitmaps with maximum 16 <span class=SpellE>colors</span>, the
best bitmaps are converted SVG files or converted vector graphic. Convert them
to GIF and reduce the <span class=SpellE>colors</span> if possible to 4 or 5 <span
class=SpellE>colors</span>.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>The bitmap
will be shown flipped and rotated below &quot;Bitmap rotation&quot;, this is
correct for the matrix.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>There are
10 possible <span class=SpellE>colors</span> (BLACK, GREEN, RED, ORANGE and
additional RANDOMCOLOR, RANDOMCOLUMNCOLOR, RANDOMLINECOLOR, RANDOMREDGREENMULTICOLOR,
MULTICOLOR, RANDOMREDORANGEMULTICOLOR). The option &quot;Common Random
Columns/Lines&quot; at the settings will be used for RANDOMCOLUMNCOLOR and RANDOMLINECOLOR
if you set this option to 1 the bitmap would be too <span class=SpellE>colorfull</span>
with 3 it looks better.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>All bitmaps
are normally set to &quot;Transparent&quot; i.e. black will not plotted except
if you want to scroll the bitmap. Therefore you can draw different bitmaps at
the same time to the matrix without destroying with the black pixels, they will
be overlaid.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>If you
imported a bitmap, the label of each used <span class=SpellE>color</span> has
the <span class=SpellE>color</span> of this <span class=SpellE>color</span>.
You can now select the <span class=SpellE>color</span> for each <span
class=SpellE>color</span>. If you don't select a <span class=SpellE>color</span>,
this <span class=SpellE>color</span> will be BLACK. After you selected all
necessary <span class=SpellE>colors</span> you can test the bitmap or add to
script.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Use Text as Bitmap<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>For Text as
Bitmap only two <span class=SpellE>colors</span> will be stored, 0 for
background and 1 for the foreground but you can use all <span class=SpellE>colors</span>
for background and foreground. <o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>With
&quot;Select Font&quot; you can select any installed font with any size and
attribute, only the <span class=GramE>number of <span class=SpellE>colors</span>
are</span> restricted.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>You can
test your text or add it to the script.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Draw<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Here you
will find all functions of <span class=SpellE>Lonewolf's</span> drawing
library.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Normal Text<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>I use only
the font FONT_5x7W because with the Arduino <span class=SpellE>Duemilanove</span>
I have restricted memory<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>These
functions are the same as <span class=SpellE>putchar</span> and <span
class=SpellE>scrolltext</span>, the Show is a function where <span
class=SpellE>putchar</span> writes a string without scrolling.<o:p></o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Special Clear/Fill Effects<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>These
functions work with testing but if you upload it and you start a scrolling
function afterward, the whole effects will be not visible. It is only a proof
of concept<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Add Clear Matrix/Send
Frame/Delay to the Script<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>If you want
to clear the matrix, show the content on the matrix or add a delay.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Matrix Script<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Now the
most important thing, it is a <span class=SpellE>datagridview</span>, similar
to a spread sheet. <o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>You can
change the rows but for bitmap and text bitmap you can't change the bitmap
data, you have to load them again.<o:p></o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Types of the Matrix Script<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Bitmap, for
scrolling a large X or Y for direction could be added or removed<o:p></o:p></span></p>

<p class=MsoNormal><span class=SpellE><span lang=EN-GB style='mso-ansi-language:
EN-GB'>TextBitmap</span></span><span lang=EN-GB style='mso-ansi-language:EN-GB'>,
for scrolling a large X or Y for direction could be added or removed. You can
change the <span class=SpellE>colors</span> at Front <span class=SpellE>Color</span>
and Background <span class=SpellE>color</span><o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Text, for
show a large X or Y for direction is necessary, for scrolling stands <span
class=SpellE>TextScroll</span> and large X or Y for direction<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Delay,
Delay in Milliseconds<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Clear,
clear the matrix<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>All other
functions are the same as written before<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Test the Matrix Script<o:p></o:p></span></h1>

<p class=MsoNormal><span class=GramE><span lang=EN-GB style='mso-ansi-language:
EN-GB'>Runs all content of the matrix script with a background worker.</span></span><span
lang=EN-GB style='mso-ansi-language:EN-GB'> Scrolling is really slow. <o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>You have to
push to &quot;Stop the Script Loop&quot; to stop the matrix loop.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Copy to SD card and run
remotely<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>This is
another failed proof of concept. The aim was that the Arduino board will be
installed remotely without a computer, only with an Ethernet shield and a SD
card to receive data over LAN.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>First the
Ethernet and SD card could not be used at the same time and second SD card
could only handle one file at the same time instead of wished 2 files (one file
for the commands, the second file for bitmap data).<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>For text
and drawing functions of <span class=SpellE>Lonewolf's</span> library it could
be used but for bitmap scrolling it would take up to 5 minutes to write, the
scrolling would not be faster than over USB and if you contact over USB, all
data will be lost.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Save Script as Text file<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>Save your
data as often you want if you &quot;Open Text Script File&quot;, the file
content will be appended to the <span class=SpellE>datagridview</span>.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

<h1><span lang=EN-GB style='mso-ansi-language:EN-GB'>Copy Script as Arduino
File to Clipboard<o:p></o:p></span></h1>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'>If you still
have Arduino IDE open but the COM port at Settings closed, you can upload the
file to your Arduino. Now you will see how fast the Arduino is.<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-GB style='mso-ansi-language:EN-GB'><o:p>&nbsp;</o:p></span></p>

</div>
