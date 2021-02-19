# Images
There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.

**Adding Images**

`<img>`


To add an image into the page
you need to use an `<img>`
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:

src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images — relative URLs
were covered on pages 83-84).

alt

This provides a text description
of the image which describes the
image if you cannot see it.


**Height & Width
 of Images**

 You will also often see an `<img>`
element use two other attributes
that specify its size:

**height**

This specifies the height of the
image in pixels.

**width**

This specifies the width of the
image in pixels.


**Where to Place Images
in Your Code**

Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:

1: before a paragraph

The paragraph starts on a new
line after the image.

2: inside the start of a
paragraph
The first row of text aligns with
the bottom of the image.

3: in the middle of a
paragraph

The image is placed between the
words of the paragraph that it
appears in.


**Aligning
Images Horizontally**

align chapter-05/aligning-images-horizontally.html HTML
The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image.

The align attribute can take
these horizontal values:

left

This aligns the image to the left
(allowing text to flow around its
right-hand side).

right

This aligns the image to the right
(allowing text to flow around its
left-hand side).

**Aligning
Images Vertically**

There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:

top

This aligns the first line of the
surrounding text with the top of
the image.

middle

This aligns the first line of the
surrounding text with the middle
of the image.

bottom

This aligns the first line of the
surrounding text with the bottom
of the image.



**Tools to Edit
& Save Images**

There are several tools you can use to edit and
save images to ensure that they are the right
size, format, and resolution.

The most popular tool amongst
web professionals is Adobe
Photoshop.


**Image Dimensions**

The images you use on your website should be
saved at the same width and height that you
want them to appear on the page.


**Cropping Images**

When cropping images it is important not to
lose valuable information. It is best to source
images that are the correct shape if possible.

**Image Resolution**

Images created for the web should be saved at
a resolution of 72 ppi. The higher the resolution
of the image, the larger the size of the file.



JPGs, GIFs, and PNGs belong to
a type of image format known
as bitmap. They are made up of
lots of miniature squares. The
resolution of an image is the
number of squares that fit within
a 1 inch x 1 inch square area.



Images appearing on computer
screens are made of tiny squares
called pixels. A small segment
of this photograph has been
magnified to show how it is
made up of pixels.


**Animated GIFs**

Animated GIFs show several frames of an
image in sequence and therefore can be used to
create simple animations.



# Color

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:


rgb values

These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)

 hex codes

These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80

color names

There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan


**Background Color**

CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.


**Understanding Color**



Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.



**CSS3: HSL & HSLA**

The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:

hue

This is expressed as an angle
(between 0 and 360 degrees).

saturation

This is expressed as a
percentage.

lightness

This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.


# Text

The properties that allow you to control
the appearance of text can be split into
two groups:

● Those that directly affect the font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text).

● Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters).

*Specifying Typefaces
font-family**

The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.


Size of Type

The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:

pixels

Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.

percentages

The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.

**font-weight**

The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:

normal

This causes text to appear at a
normal weight.

bold

This causes text to appear bold.

**font-style**

If you want to create italic text,
you can use the font-style
property. There are three values
this property can take:

normal

This causes text to appear in a
normal style (as opposed to italic
or oblique).

italic

This causes text to appear italic.

oblique

This causes text to appear
oblique.




**text-transform**

The text-transform property
is used to change the case of
text giving it one of the following
values:

uppercase

This causes the text to appear
uppercase.

lowercase

This causes the text to appear
lowercase.

capitalize

This causes the first letter of
each word to appear capitalized.



**text-decoration**

The text-decoration property
allows you to specify the
following values:

none

This removes any decoration
already applied to the text.

underline

This adds a line underneath the
text.

overline

This adds a line over the top of
the text.

line-through

This adds a line through words.

blink

This animates the text to make it
flash on and off (however this is
generally frowned upon, as it is
considered rather annoying).


**line-height**

Leading (pronounced ledding) is
a term typographers use for the
vertical space between lines of
text. 

**text-align**

The text-align property allows
you to control the alignment of
text. The property can take one
of four values:

left

This indicates that the text
should be left-aligned.

right

This indicates that the text
should be right-aligned.

center

This allows you to center text.

justify

This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.

**vertical-align**

The vertical-align property is
a common source of confusion.
It is not intended to allow you to
vertically align text in the middle
of block level elements such as
`<p>` and `<div>`, although it does
have this effect when used with
table cells (the `<td>` and `<th>`
elements).

**text-indent**
The text-indent property
allows you to indent the first
line of text within an element.
The amount you want the line
indented by can be specified in
a number of ways but is usually
given in pixels or ems.

**text-shadow**

he text-shadow property has
become commonly used despite
lacking support in all browsers.
It is used to create a drop
shadow, which is a dark version
of the word just behind it and
slightly offset. It can also be used
to create an embossed effect by
adding a shadow that is slightly
lighter than the text.


The value of this property is
quite complicated because it can
take three lengths and a color for
the drop shadow.

The first length indicates how
far to the left or right the shadow
should fall.

The second value indicates the
distance to the top or bottom
that the shadow should fall.

The third value is optional and
specifies the amount of blur that
should be applied to the drop
shadow.

The fourth value is the color of
the drop shadow.


**First Letter or Line**

You can specify different values
for the first letter or first line of
text inside an element using
:first-letter and
:first-line.

Technically these are not
properties. They are known as
pseudo-elements.

**Styling Links**

rowsers tend to show links
in blue with an underline by
default, and they will change
the color of links that have been
visited to help users know which
pages they have been to.

In CSS, there are two pseudoclasses that allow you to set
different styles for links that
have and have not yet been
visited.

:link

This allows you to set styles
for links that have not yet been
visited.

:visited

This allows you to set styles for
links that have been clicked on.
They are commonly used to
control colors of the links and
also whether they are to appear
underlined or not.


**Responding to Users**


There are three pseudo-classes
that allow you to change the
appearance of elements when a
user is interacting with them.

:hover

This is applied when a user
hovers over an element with a
pointing device such as a mouse.
This has commonly been used
to change the appearance of
links and buttons when a user
places their cursor over them. It
is worth noting that such events
do not work on devices that use
touch screens (such as the iPad)
because the screen is not able to
tell when someone is hovering
their finger over an element.

:active

This is applied when an element
is being activated by a user; for
example, when a button is being
pressed or a link being clicked.
Sometimes this is used to make
a button or link feel more like it
is being pressed by changing the
style or position of the element
slightly.

:focus

This is applied when an element
has focus. Any element that
you can interact with, such as a
link you can click on or any form
control can have focus.




# JPEG vs PNG vs GIF — which image format to use and when?

**Compression**

Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.

Compression can be of two types — lossless and lossy. In lossless compression, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression. This is not the case in lossy compression i.e. data loss in lossy compression is irreversible. Lossy compression algorithms always have a superior compression ratio (the ratio of size of compressed image to original image) as compared to lossless compression. However, this compression ratio comes at a cost of reduced quality that becomes more evident after zooming in on the image. This noticeable reduction in quality or distortion of the image is called compression artefact.



JPEG is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality. Beyond this, the compression artefacts become more prominent. Because JPEG compression works by averaging out colours of nearby pixels (read Discrete Cosine Transform), JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth. However, if an image contains text or lines, where a sharp contrast between adjacent pixels is desired to highlight the proper shape, this lossy compression technique does not yield good results.


PNG is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.


GIF is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.



**Transparency**

In a simple form, transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.

JPEG images don’t support transparency and are hence not usable for such cases.
PNG images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency). Partial transparency makes the edges blend smoothly into the background. PNG8 images (discussed in the “Colours” section below) can support only index transparency whereas PNG24 images can support alpha channel transparency.

GIF images support transparency by declaring a single colour in the colour palette as transparent (index transparency). Because of absence of partial transparency, the edges (specially rounded or too-detailed edges) get a poor jagged effect. Though this can be solved to some extent using dithering, with improved PNG support, GIF is unsuitable for images with transparent backgrounds.


**Colours**

There is a significant difference in the number of colours that can be supported by these 3 formats.
JPEG images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

PNG images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.

GIF images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.


**Animation**

Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time.
Of these 3 formats, only GIF supports animation. This capability makes GIF format suitable for delivering engaging ads and banners. Of late, with the advent of companies Tumblr, 9Gag, Giphy etc. the use of GIF format for memes has picked up.


These are some of the major differences between the three most popular image formats for web — JPEG, PNG and GIF. To summarise once again, use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.


