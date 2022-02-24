Canvas size: 750 x 1624
Features present: animation transparency
Background color : 0xFFFFFFFF  Loop Count : 0
Number of frames: 50
No.: width height alpha x_offset y_offset duration   dispose blend image_size  compression
  1:   750  1624   yes        0        0      100       none    no     105034       lossy
  2:   750  1624   yes        0        0      100 background    no     101890       lossy
  3:   484  1624   yes      266        0      100       none    no      60934       lossy
  4:   750  1624   yes        0        0      100 background    no      85834       lossy
  5:   750  1494   yes        0      130      100       none    no      63380       lossy
  6:   750  1580   yes        0       44      100       none    no      65572       lossy
  7:   750  1624   yes        0        0      100       none    no      72442       lossy
  8:   750  1624   yes        0        0      100       none    no      73694       lossy
  9:   750  1624   yes        0        0      100       none    no      71878       lossy
 10:   750  1624   yes        0        0      100       none    no      69672       lossy
 11:   750  1624   yes        0        0      100       none    no      68746       lossy
 12:   750  1624   yes        0        0      100       none    no      68856       lossy
 13:   750  1624   yes        0        0      100       none    no      69048       lossy
 14:   750  1624   yes        0        0      100       none    no      69186       lossy
 15:   750  1624   yes        0        0      100       none    no      68756       lossy
 16:   750  1624   yes        0        0      100       none    no      82274       lossy
 17:   750  1624   yes        0        0      100 background    no     186288       lossy
 18:   604  1624   yes        0        0      100 background    no     129336       lossy
 19:   134   426   yes        0     1198      100 background    no      10114       lossy
 20:    15    63   yes        0     1460      100 background    no        484       lossy
 21:   404   402   yes        0      404      100       none    no      18342       lossy
 22:   620   492   yes        0      404      100 background    no      33722       lossy
 23:   750   725   yes        0      436      100       none    no      43152       lossy
 24:   750   899   yes        0      354      100       none    no      34062       lossy
 25:   750   928   yes        0      340      100       none    no      34610       lossy
 26:   750   940   yes        0      334      100       none    no      34434       lossy
 27:   750   957   yes        0      328      100       none    no      33994       lossy
 28:   750   976   yes        0      320      100       none    no      33204       lossy
 29:   750   993   yes        0      314      100       none    no      33316       lossy
 30:   750  1012   yes        0      306      100       none    no      32864       lossy
 31:   750  1027   yes        0      302      100       none    no      32536       lossy
 32:   750  1624   yes        0        0      100       none    no     129458       lossy
 33:   750  1624   yes        0        0      100       none   yes       6866       lossy
 34:   750  1624   yes        0        0      100       none    no       8260       lossy
 35:   750  1624   yes        0        0      100       none    no     147428       lossy
 36:   750  1624   yes        0        0      100       none    no      28958       lossy
 37:   750  1624   yes        0        0      100       none    no     238378       lossy
 38:   750  1624   yes        0        0      100       none    no     314272       lossy
 39:   750  1624   yes        0        0      100       none    no     317232       lossy
 40:   750  1624   yes        0        0      100       none    no     253550       lossy
 41:   750  1624   yes        0        0      100       none    no     229756       lossy
 42:   750  1624   yes        0        0      100       none    no     186178       lossy
 43:   750  1624   yes        0        0      100       none    no     146924       lossy
 44:   750  1624   yes        0        0      100       none    no     115494       lossy
 45:   750  1624   yes        0        0      100       none    no      65626       lossy
 46:   507   529   yes      122      462      100       none    no      61570       lossy
 47:   535   560   yes      108      452      100       none    no      64116       lossy
 48:   504   537   yes      124      462      100       none    no      61726       lossy
 49:   535   560   yes      108      452      100       none    no      63972       lossy
 50:   535   560   yes      108      452      100       none    no      63888       lossy
Usage: webpmux -get GET_OPTIONS INPUT -o OUTPUT
       webpmux -set SET_OPTIONS INPUT -o OUTPUT
       webpmux -duration DURATION_OPTIONS [-duration ...]
               INPUT -o OUTPUT
       webpmux -strip STRIP_OPTIONS INPUT -o OUTPUT
       webpmux -frame FRAME_OPTIONS [-frame...] [-loop LOOP_COUNT]
               [-bgcolor BACKGROUND_COLOR] -o OUTPUT
       webpmux -info INPUT
       webpmux [-h|-help]
       webpmux -version
       webpmux argument_file_name

GET_OPTIONS:
 Extract relevant data:
   icc       get ICC profile
   exif      get EXIF metadata
   xmp       get XMP metadata
   frame n   get nth frame

SET_OPTIONS:
 Set color profile/metadata/parameters:
   loop LOOP_COUNT            set the loop count
   bgcolor BACKGROUND_COLOR   set the animation background color
   icc  file.icc              set ICC profile
   exif file.exif             set EXIF metadata
   xmp  file.xmp              set XMP metadata
   where:    'file.icc' contains the ICC profile to be set,
             'file.exif' contains the EXIF metadata to be set
             'file.xmp' contains the XMP metadata to be set

DURATION_OPTIONS:
 Set duration of selected frames:
   duration            set duration for each frames
   duration,frame      set duration of a particular frame
   duration,start,end  set duration of frames in the
                        interval [start,end])
   where: 'duration' is the duration in milliseconds
          'start' is the start frame index
          'end' is the inclusive end frame index
           The special 'end' value '0' means: last frame.

STRIP_OPTIONS:
 Strip color profile/metadata:
   icc       strip ICC profile
   exif      strip EXIF metadata
   xmp       strip XMP metadata

FRAME_OPTIONS(i):
 Create animation:
   file_i +di+[xi+yi[+mi[bi]]]
   where:    'file_i' is the i'th animation frame (WebP format),
             'di' is the pause duration before next frame,
             'xi','yi' specify the image offset for this frame,
             'mi' is the dispose method for this frame (0 or 1),
             'bi' is the blending method for this frame (+b or -b)

LOOP_COUNT:
 Number of times to repeat the animation.
 Valid range is 0 to 65535 [Default: 0 (infinite)].

BACKGROUND_COLOR:
 Background color of the canvas.
  A,R,G,B
  where:    'A', 'R', 'G' and 'B' are integers in the range 0 to 255 specifying
            the Alpha, Red, Green and Blue component values respectively
            [Default: 255,255,255,255]

INPUT & OUTPUT are in WebP format.

Note: The nature of EXIF, XMP and ICC data is not checked and is assumed to be
valid.

Note: if a single file name is passed as the argument, the arguments will be
tokenized from this file. The file name must not start with the character '-'.
