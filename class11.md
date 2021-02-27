# Images

Controlling the size and alignment of
your images using CSS keeps rules that
affect the presentation of your page in
the CSS and out of the HTML markup.

**Controlling sizes of images in CSS**

You can control the size of an
image using the width and
height properties in CSS, just
like you can for any other box.


**AligNing images Using CSS**

the
align-left and align-right
classes used to align the image.


**Centering images Using CSS**

In order to center an image, it
should be turned into a blocklevel element using the display
property with a value of block.

Once it has been made into a
block-level element, there are
two common ways in which you
can horizontally center an image:

1: On the containing element,
you can use the text-align
property with a value of center.

2: On the image itself, you can
use the use the margin property
and set the values of the left and
right margins to auto.



**Background Images**

The background-image
property allows you to place
an image behind any HTML
element. This could be the entire
page or just part of the page. By
default, a background image will
repeat to fill the entire box.



**Repeating Images**

The background-repeat
property can have four values:

repeat

The background image is
repeated both horizontally and
vertically (the default way it
is shown if the backgroundrepeat property isn't used).

repeat-x

The image is repeated
horizontally only (as shown in
the first example on the left).

repeat-y

The image is repeated vertically
only.

no-repeat

The image is only shown once.
The background-attachment
property specifies whether a
background image should stay in
one position or move as the user
scrolls up and down the page. It
can have one of two values:

fixed

The background image stays in
the same position on the page.

scroll

The background image moves
up and down as the user scrolls
up and down the page.


**Background Position**

When an image is not being
repeated, you can use the
background-position
property to specify where in the
browser window the background
image should be placed.


This property usually has a pair
of values. The first represents
the horizontal position and the
second represents the vertical.


**shorthand background**

The background property acts
like a shorthand for all of the
other background properties
you have just seen, and also the
background-color property.


The properties must be specified
in the following order, but you
can miss any value if you do not
want to specify it.


1: background-color

2: background-image

3: background-repeat

4: background-attachment

5: background-position


**Image Rollovers & Sprites**

Using CSS, it is possible to create
a link or button that changes to a
second style when a user moves
their mouse over it (known as a
rollover) and a third style when
they click on it.


This is achieved by setting a
background image for the link or
button that has three different
styles of the same button (but
only allows enough space to
show one of them at a time).


**CSS3: Gradients**

CSS3 is going to introduce the
ability to specify a gradient for
the background of a box. The
gradient is created using the
background-image property
and, at the time of writing,
different browsers required a
different syntax.


Since it is not supported by all
browsers, it is possible to specify
a background image for the box
first (which would represent the
gradient) and then provide the
CSS alternatives for browsers
that support gradients.



**Contrast of background images**

If you want to overlay text on a background image, the image must be low
contrast in order for the text to be legible.


High Contrast

The majority of photographs
have quite a high contrast, which
means that they are not ideal for
use as a background image.


Low Contrast

Image editing applications such
as Photoshop and GIMP have
tools that allow you to manually
adjust your images to have lower
contrast.


Screen

To overlay text on an image with
high contrast, you can place a
semi-transparent background
color (or "screen") behind the
text to improve legibility.


# Practical Information

Search Engine Optimization (SEO)

SEO is a huge topic and several books have been written on the subject.
The following pages will help you understand the key concepts so you can
improve your website's visibility on search engines.


On-Page SEO

In every page of your website there are seven key places where keywords
(the words people might search on to find your site) can appear in order
to improve its findability.


1: Page Title

The page title appears at the top
of the browser window or on the
tab of a browser. It is specified in
the <title> element which lives
inside the <head> element.


2: URL / Web Address

The name of the file is part of
the URL. Where possible, use
keywords in the file name.


3: Headings

If the keywords are in a heading
`<hn>` element then a search
engine will know that this page is
all about that subject and give it
greater weight than other text.

4: Text

Where possible, it helps to
repeat the keywords in the main
body of the text at least 2-3
times. Do not, however, over-use
these terms, because the text
must be easy for a human to
read.


5: Link Text

Use keywords in the text that
create links between pages
(rather than using generic
expressions such as "click here").


6: Image Alt Text

Search engines rely on you
providing accurate descriptions
of images in the alt text. This
will also help your images show
up in the results of image-based
searches.


7: Page Descriptions

The description also lives inside
the `<head>` element and is
specified using a `<meta>` tag.
It should be a sentence that
describes the content of the
page. (These are not shown in
the browser window but they
may be displayed in the results
pages of search engines.)


**How to Identify Keywords and Phrases**

Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO. Here are six steps that
will help you identify the right keywords and phrases for your site.


1: Brainstorm

List down the words that
someone might type into
Google to find your site. Be sure
to include the various topics,
products or services your site is
about.


2: Organize

Group the keywords into
separate lists for the different
sections or categories of your
website.

3: Research

There are several tools that let
you enter your keywords and
then they will suggest additional
keywords you might like to
consider, such as:
adwords.google.co.uk/
select/KeywordToolExternal
(When using this tool, select the
"exact match" option rather than
"broad match.")
www.wordtracker.com
www.keyworddiscovery.com
Once these tools have suggested
additional keywords, add the
relevant options to your lists.
(Keyword tools will most likely
suggest some terms that are
irrelevant so do omit any that do
not seem appropriate).




4: Compare

It is very unlikely that your
site will appear at the top of
the search results for every
keyword. This is especially true
for topics where there is a lot
of competition. The more sites
out there that have already been
optimized for a given keyword,
the harder it will be for you to
rise up the search results when
people search on that term.


5: Refine

Now you need to pick which
keywords you will focus on.
These should always be the ones
that are most relevant to each
section of your site.




6: Map

Now that you have a refined list
of keywords, you know which
have the most competition, and
which ones are most relevant,
it is time to start picking which
keywords you will use for each
page.


**Analytics: Learning about your Visitors**

As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are
leaving. One of the best tools for doing this is a free service offered by
Google called Google Analytics.

Signing Up

The Google Analytics service
relies on you signing up for an
account at:
www.google.com/analytics
The site will give you a piece of
tracking code which you need to
put on every page of your site.



How it Works

Every time someone loads a
page of your site, the tracking
code sends data to the Google
servers where it is stored.
Google then provides a webbased interface that allows you
to see how visitors use your site.




The Tracking Code

A tracking code is provided
by Google Analytics for each
website you are tracking. It
should appear just before the
closing `</head>` tag. The code
does not alter the appearance of
your web pages.





**How Many People Are Coming to Your Site?**


The overview page gives you a snapshot of the key information you are
likely to want to know. In particular, it tells you how many people are
coming to your site.


Visits

This is the number of times
people have come to your site. If
someone is inactive on your site
for 30 minutes and then looks at
another page on your site, it will
be counted as a new visit.


Unique Visits

This is the total number of
people who have visited your site
over the specified period. The
number of unique visits will be
lower than the number of visits
if people have been returning to
your site more than once in the
defined period.





Page Views

The total number of pages all
visitors have viewed on your site.

Pages per Visit

The average number of pages
each visitor has looked at on
your site per visit.

Average Time on Site

The average amount of time
each user has spent on the site
per visit.

Date Selector

Using the date selector in the top
right hand corner of the site, you
can change the period of time
the reports display. When you
log in, this is usually set to the
last month, but you can change
it to report on a specific time
period.

Export

The export link just above the
title that says "visitors overview"
allows you to export the
statistics on this page for other
applications such as Excel.


**What Are Your Visitors Looking At?**

The content link on the left-hand side allows
you to learn more about what the visitors are
looking at when they come to your site.


**Where Are Your Visitors Coming From?**

The traffic sources link on the left hand side
allows you to learn where your visitors are
coming from.



**Domain Names & Hosting**

In order to put your site on the web you will
need a domain name and web hosting.

DOMAIN NAMES WEB 

Your domain name is your web
address (e.g. google.com or bbc.
co.uk). There are many websites
that allow you to register domain
names. Usually you will have to
pay an annual fee to keep that
domain name.


WEB HOSTING 
So that other people can see
your site, you will need to upload
it to a web server. Web servers
are special computers that are
constantly connected to the
Internet. They are specially set
up to serve web pages when
they are requested.


**FTP & Third Party Tools**

To transfer your code and images from your
computer to your hosting company, you use
something known as File Transfer Protocol.



















