WeasyPrint changelog
====================


Version 0.32r
-------------

* Remove dependency to html5lib as its unnecessary.

Version 0.31
------------

Released on 2016-08-28.

New features:

* `#124 <https://github.com/Kozea/WeasyPrint/issues/124>`_:
  Add MIME sniffing for images.
* `#60 <https://github.com/Kozea/WeasyPrint/issues/60>`_:
  CSS Multi-column Layout.
* `#197 <https://github.com/Kozea/WeasyPrint/pull/197>`_:
  Add hyphens at line breaks activated by a soft hyphen.

Bux fixes:

* `#132 <https://github.com/Kozea/WeasyPrint/pull/132>`_:
  Fix Python 3 compatibility on Windows.

Documentation:

* `#329 <https://github.com/Kozea/WeasyPrint/issues/329>`_:
  Add documentation about installation on Windows.


Version 0.30
------------

Released on 2016-07-18.

WeasyPrint now depends on html5lib-0.999999999.

Bux fixes:

* Fix Acid2
* `#325 <https://github.com/Kozea/WeasyPrint/issues/325>`_:
  Cutting lines is broken in page margin boxes.
* `#334 <https://github.com/Kozea/WeasyPrint/issues/334>`_:
  Newest html5lib 0.999999999 breaks rendering.


Version 0.29
------------

Released on 2016-06-17.

Bug fixes:

* `#263 <https://github.com/Kozea/WeasyPrint/pull/263>`_:
  Don't crash with floats with percents in positions.
* `#323 <https://github.com/Kozea/WeasyPrint/pull/323>`_:
  Fix CairoSVG 2.0 pre-release dependency in Python 2.x.


Version 0.28
------------

Released on 2016-05-16.

Bug fixes:

* `#189 <https://github.com/Kozea/WeasyPrint/issues/189>`_:
  ``white-space: nowrap`` still wraps on hyphens
* `#305 <https://github.com/Kozea/WeasyPrint/issues/305>`_:
  Fix crashes on some tables
* Don't crash when transform matrix isn't invertible
* Don't crash when rendering ratio-only SVG images
* Fix margins and borders on some tables


Version 0.27
------------

Released on 2016-04-08.

New features:

* `#295 <https://github.com/Kozea/WeasyPrint/pull/295>`_:
  Support the 'rem' unit.
* `#299 <https://github.com/Kozea/WeasyPrint/pull/299>`_:
  Enhance the support of SVG images.

Bug fixes:

* `#307 <https://github.com/Kozea/WeasyPrint/issues/307>`_:
  Fix the layout of cells larger than their tables.

Documentation:

* The website is now on GitHub Pages, the documentation is on Read the Docs.
* `#297 <https://github.com/Kozea/WeasyPrint/issues/297>`_:
  Rewrite the CSS chapter of the documentation.


Version 0.26
------------

Released on 2016-01-29.

New features:

* Support the `empty-cells` attribute.
* Respect table, column and cell widths.

Bug fixes:

* `#172 <https://github.com/Kozea/WeasyPrint/issues/172>`_:
  Unable to set table column width on tables td's.
* `#151 <https://github.com/Kozea/WeasyPrint/issues/151>`_:
  Table background colour bleeds beyond table cell boundaries.
* `#260 <https://github.com/Kozea/WeasyPrint/issues/260>`_:
  TypeError: unsupported operand type(s) for +: 'float' and 'str'.
* `#288 <https://github.com/Kozea/WeasyPrint/issues/288>`_:
  Unwanted line-breaks in bold text.
* `#286 <https://github.com/Kozea/WeasyPrint/issues/286>`_:
  AttributeError: 'Namespace' object has no attribute 'attachments'.


Version 0.25
------------

Released on 2015-12-17.

New features:

* Support the 'q' unit.

Bug fixes:

* `#285 <https://github.com/Kozea/WeasyPrint/issues/285>`_:
  Fix a crash happening when splitting lines.
* `#284 <https://github.com/Kozea/WeasyPrint/issues/284>`_:
  Escape parenthesis in PDF links.
* `#280 <https://github.com/Kozea/WeasyPrint/pull/280>`_:
  Replace utf8 with utf-8 for gettext/django compatibility.
* `#269 <https://github.com/Kozea/WeasyPrint/pull/269>`_:
  Add support for use when frozen.
* `#250 <https://github.com/Kozea/WeasyPrint/issues/250>`_:
  Don't crash when attachments are not available.


Version 0.24
------------

Released on 2015-08-04.

New features:

* `#174 <https://github.com/Kozea/WeasyPrint/issues/174>`_:
  Basic support for Named strings.

Bug fixes:

* `#207 <https://github.com/Kozea/WeasyPrint/issues/207>`_:
  Draw rounded corners on replaced boxes.
* `#224 <https://github.com/Kozea/WeasyPrint/pull/224>`_:
  Rely on the font size for rounding bug workaround.
* `#31 <https://github.com/Kozea/WeasyPrint/issues/31>`_:
  Honor the vertical-align property in fixed-height cells.
* `#202 <https://github.com/Kozea/WeasyPrint/issues/202>`_:
  Remove unreachable area/border at bottom of page.
* `#225 <https://github.com/Kozea/WeasyPrint/issues/225>`_:
  Don't allow unknown units during line-height validation.
* Fix some wrong conflict resolutions for table borders with inset
  and outset styles.


Version 0.23
------------

Released on 2014-09-16.

Bug fixes:

* `#196 <https://github.com/Kozea/WeasyPrint/issues/196>`_:
  Use the default image sizing algorithm for images’s preferred size.
* `#194 <https://github.com/Kozea/WeasyPrint/pull/194>`_:
  Try more library aliases with ``dlopen()``.
* `#201 <https://github.com/Kozea/WeasyPrint/pull/201>`_:
  Consider ``page-break-after-avoid`` when pushing floats to the next page.
* `#217 <https://github.com/Kozea/WeasyPrint/issues/217>`_:
  Avoid a crash on zero-sized background images.

Release process:

* Start testing on Python 3.4 on Travis-CI.


Version 0.22
------------

Released on 2014-05-05.

New features:

* `#86 <https://github.com/Kozea/WeasyPrint/pull/86>`_:
  Support gzip and deflate encoding in HTTP responses
* `#177 <https://github.com/Kozea/WeasyPrint/pull/177>`_:
  Support for PDF attachments.

Bug fixes:

* `#169 <https://github.com/Kozea/WeasyPrint/issues/169>`_:
  Fix a crash on percentage-width columns in an auto-width table.
* `#168 <https://github.com/Kozea/WeasyPrint/issues/168>`_:
  Make ``<fieldset>`` a block in the user-agent stylesheet.
* `#175 <https://github.com/Kozea/WeasyPrint/issues/175>`_:
  Fix some ``dlopen()`` library loading issues on OS X.
* `#183 <https://github.com/Kozea/WeasyPrint/issues/183>`_:
  Break to the next page before a float that would overflow the page.
0.32r (2016-09-06)
* `#188 <https://github.com/Kozea/WeasyPrint/issues/188>`_:
  Require a recent enough version of Pyphen

Release process:

* Drop Python 3.1 support.
* Set up [Travis CI](http://travis-ci.org/)
  to automatically test all pushes and pull requests.
* Start testing on Python 3.4 locally. (Travis does not support 3.4 yet.)


Version 0.21
------------

Released on 2014-01-11.

New features:

* Add the `overflow-wrap <http://dev.w3.org/csswg/css-text/#overflow-wrap>`_
  property, allowing line breaks inside otherwise-unbreakable words.
  Thanks Frédérick Deslandes!
* Add the `image-resolution
  <http://dev.w3.org/csswg/css-images-3/#the-image-resolution>`_ property,
  allowing images to be sized proportionally to their intrinsic size
  at a resolution other than 96 image pixels per CSS ``in``
  (ie. one image pixel per CSS ``px``)

Bug fixes:

* `#145 <https://github.com/Kozea/WeasyPrint/issues/145>`_:
  Fix parsing HTML from an HTTP URL on Python 3.x
* `#40 <https://github.com/Kozea/WeasyPrint/issues/40>`_:
  Use more general hyphenation dictionnaries for specific document languages.
  (E.g. use ``hyph_fr.dic`` for ``lang="fr_FR"``.)
* `#26 <https://github.com/Kozea/WeasyPrint/issues/26>`_:
  Fix ``min-width`` and ``max-width`` on floats.
* `#100 <https://github.com/Kozea/WeasyPrint/issues/100>`_:
  Fix a crash on trailing whitespace with ``font-size: 0``
* `#82 <https://github.com/Kozea/WeasyPrint/issues/82>`_:
  Borders on tables with ``border-collapse: collapse`` were sometimes
  drawn at an incorrect position.
* `#30 <https://github.com/Kozea/WeasyPrint/issues/30>`_:
  Fix positioning of images with ``position: absolute``.
* `#118 <https://github.com/Kozea/WeasyPrint/issues/118>`_:
  Fix a crash when using ``position: absolute``
  inside a ``position: relative`` element.
* Fix ``visibility: collapse`` to behave like ``visibility: hidden``
  on elements other than table rows and table columns.
* `#147 <https://github.com/Kozea/WeasyPrint/issues/147>`_ and
  `#153 <https://github.com/Kozea/WeasyPrint/issues/153>`_:
  Fix dependencies to require lxml 3.0 or a more recent version.
  Thanks gizmonerd and Thomas Grainger!
* `#152 <https://github.com/Kozea/WeasyPrint/issues/152>`_:
  Fix a crash on percentage-sized table cells in auto-sized tables.
  Thanks Johannes Duschl!


Version 0.20.2
--------------

Released on 2013-12-18.

* Fix `#146 <https://github.com/Kozea/WeasyPrint/issues/146>`_: don't crash
  when drawing really small boxes with dotted/dashed borders


Version 0.20.1
--------------

Released on 2013-12-16.

* Depend on html5lib >= 0.99 instead of 1.0b3 to fix pip 1.4 support.
* Fix `#74 <https://github.com/Kozea/WeasyPrint/issues/74>`_: don't crash on
  space followed by dot at line break.
* Fix `#78 <https://github.com/Kozea/WeasyPrint/issues/78>`_: nicer colors for
  border-style: ridge/groove/inset/outset.


Version 0.20
------------

Released on 2013-12-14.

* Add support for ``border-radius``.
* Feature `#77 <https://github.com/Kozea/WeasyPrint/issues/77>`_: Add PDF
  metadata from HTML.
* Feature `#12 <https://github.com/Kozea/WeasyPrint/pull/12>`_: Use html5lib.
* Tables: handle percentages for column groups, columns and cells, and values
  for row height.
* Bug fixes:

  * Fix `#84 <https://github.com/Kozea/WeasyPrint/pull/84>`_: don't crash when
    stylesheets are not available.
  * Fix `#101 <https://github.com/Kozea/WeasyPrint/issues/101>`_: use page ids
    instead of page numbers in PDF bookmarks.
  * Use ``logger.warning`` instead of deprecated ``logger.warn``.
  * Add 'font-stretch' in the 'font' shorthand.


Version 0.19.2
--------------

Released on 2013-06-18.

Bug fix release:

* Fix `#88 <https://github.com/Kozea/WeasyPrint/issues/88>`_:
  ``text-decoration: overline`` not being drawn above the text
* Bug fix: Actually draw multiple lines when multiple values are given
  to ``text-decoration``.
* Use the font metrics for text decoration positioning.
* Bug fix: Don't clip the border with ``overflow: hidden``.
* Fix `#99 <https://github.com/Kozea/WeasyPrint/issues/99>`_:
  Regression: JPEG images not loading with cairo 1.8.x.


Version 0.19.1
--------------

Released on 2013-04-30.

Bug fix release:

* Fix incorrect intrinsic width calculation
  leading to unnecessary line breaks in floats, tables, etc.
* Tweak border painting to look better
* Fix unnecessary page break before big tables.
* Fix table row overflowing at the bottom of the page
  when there are margins above the table.
* Fix ``position: fixed`` to actually repeat on every page.
* Fix `#76 <https://github.com/Kozea/WeasyPrint/issues/76>`_:
  repeat ``<thead>`` and ``<tfoot>`` elements on every page,
  even with table border collapsing.


Version 0.19
------------

Released on 2013-04-18.

* Add support for ``linear-gradient()`` and ``radial-gradient``
  in background images.
* Add support for the ``ex`` and ``ch`` length units.
  (``1ex`` is based on the font instead of being always ``0.5em`` as before.)
* Add experimental support for Level 4 hyphenation properties.
* Drop support for CFFI < 0.6 and cairocffi < 0.4.
* Many bug fixes, including:

 * Fix `#54 <https://github.com/Kozea/WeasyPrint/issues/54>`_:
   min/max-width/height on block-level images.
 * Fix `#71 <https://github.com/Kozea/WeasyPrint/issues/71>`_:
   Crash when parsing nested functional notation.


Version 0.18
------------

Released on 2013-03-30.

* Add support for Level 3 backgrounds,
  including multiple background layers per element/box.
* Forward-compatibility with (future releases of) cairocffi 0.4+ and CFFI 0.6+.
* Bug fixes:

  * Avoid some unnecessary line breaks
    for elements sized based on their content (aka. “shrink-to-fit”)
    such as floats and page headers.
  * Allow page breaks between empty blocks.
  * Fix `#66 <https://github.com/Kozea/WeasyPrint/issues/66>`_:
    Resolve images’ auto width from non-auto height and intrinsic ratio.
  * Fix `#21 <https://github.com/Kozea/WeasyPrint/issues/21>`_:
    The ``data:`` URL scheme is case-insensitive.
  * Fix `#53 <https://github.com/Kozea/WeasyPrint/issues/53>`_:
    Crash when backtracking for ``break-before/after: avoid``.


Version 0.17.1
--------------

Released on 2013-03-18.

Bug fixes:

* Fix `#41 <https://github.com/Kozea/WeasyPrint/issues/41>`_:
  GObject initialization when GDK-PixBuf is not installed.
* Fix `#42 <https://github.com/Kozea/WeasyPrint/issues/42>`_:
  absolute URLs without a base URL (ie. document parsed from a string.)
* Fix some whitespace collapsing bugs.
* Fix absolutely-positioned elements inside inline elements.
* Fix URL escaping of image references from CSS.
* Fix `#49 <https://github.com/Kozea/WeasyPrint/issues/49>`_:
  Division by 0 on dashed or dotted border smaller than one dot/dash.
* Fix `#44 <https://github.com/Kozea/WeasyPrint/issues/44>`_:
  bad interaction of ``page-break-before/after: avoid`` and floats.


Version 0.17
------------

Released on 2013-02-27.

* Added `text hyphenation`_ with the ``-weasy-hyphens`` property.
* When a document includes JPEG images, embed them as JPEG in the PDF output.
  This often results in smaller PDF file size
  compared to the default *deflate* compression.
* Switched to using CFFI instead of PyGTK or PyGObject-introspection.
* Layout bug fixes:

  - Correctly trim whitespace at the end of lines.
  - Fix some cases with floats within inline content.

.. _text hyphenation: http://weasyprint.org/docs/features/#hyphenation


Version 0.16
------------

Released on 2012-12-13.

* Add the :obj:`zoom` parameter to :meth:`HTML.write_pdf` and
  :meth:`Document.write_pdf() <weasyprint.document.Document.write_pdf>`
* Fix compatibility with old (and buggy) pycairo versions.
  WeasyPrint is now tested on 1.8.8 in addition to the latest.
* Fix layout bugs related to line trailing spaces.


Version 0.15
------------

Released on 2012-10-09.

* Add a low-level API that enables painting pages individually on any
  cairo surface.
* **Backward-incompatible change**: remove the :meth:`HTML.get_png_pages`
  method. The new low-level API covers this functionality and more.
* Add support for the ``font-stretch`` property.
* Add support for ``@page:blank`` to select blank pages.
* New Sphinx-based and improved docs
* Bug fixes:

  - Importing Pango in some PyGTK installations.
  - Layout of inline-blocks with `vertical-align: top` or `bottom`.
  - Do not repeat a block’s margin-top or padding-top after a page break.
  - Performance problem with large tables split across many pages.
  - Anchors and hyperlinks areas now follow CSS transforms.
    Since PDF links have to be axis-aligned rectangles, the bounding box
    is used. This may be larger than expected with rotations that are
    not a multiple of 90 degrees.


Version 0.14
------------

Released on 2012-08-03.

* Add a public API to choose media type used for @media.
  (It still defaults to ``print``). Thanks Chung Lu!
* Add ``--base-url`` and ``--resolution`` to the command-line API, making it
  as complete as the Python one.
* Add support for the ``<base href="...">`` element in HTML.
* Add support for CSS outlines
* Switch to gdk-pixbuf instead of Pystacia for loading raster images.
* Bug fixes:

  - Handling of filenames and URLs on Windows
  - Unicode filenames with older version of py2cairo
  - ``base_url`` now behaves as expected when set to a directory name.
  - Make some tests more robust


Version 0.13
------------

Released on 2012-07-23.

* Add support for PyGTK, as an alternative to PyGObject + introspection.
  This should make WeasyPrint easier to run on platforms that not not have
  packages for PyGObject 3.x yet.
* Bug fix: crash in PDF outlines for some malformed HTML documents


Version 0.12
------------

Released on 2012-07-19.

* Add support for collapsed borders on tables. This is currently incompatible
  with repeating header and footer row groups on each page: headers and footers
  are treated as normal row groups on table with ``border-collapse: collapse``.
* Add ``url_fetcher`` to the public API. This enables users to hook into
  WeasyPrint for fetching linked stylesheets or images, eg. to generate them
  on the fly without going through the network.
  This enables the creation of `Flask-WeasyPrint
  <http://packages.python.org/Flask-WeasyPrint/>`_.


Version 0.11
------------

Released on 2012-07-04.

* Add support for floats and clear.
  Together with various bug fixes, this enables WeasyPrint to pass the Acid2
  test! Acid2 is now part of our automated test suite.
* Add support for the width, min-width, max-width, height, min-height and
  max-height properties in @page. The size property is now the size of the
  page’s containing block.
* Switch the Variable Dimension rules to `the new proposal
  <https://github.com/SimonSapin/css/blob/master/margin-boxes-variable-dimension>`_.
  The previous implementation was broken in many cases.
* The ``image-rendering``, ``transform``, ``transform-origin`` and ``size``
  properties are now unprefixed. The prefixed form (eg. -weasy-size) is ignored
  but gives a specific warning.


Version 0.10
------------

Released on 2012-06-25.

* Add ``get_png_pages()`` to the public API. It returns each page as
  a separate PNG image.
* Add a ``resolution`` parameter for PNG.
* Add *WeasyPrint Navigator*, a web application that shows WeasyPrint’s
  output with clickable links. Yes, that’s a browser in your browser.
  Start it with ``python -m weasyprint.navigator``
* Add support for `vertical-align: top` and `vertical-align: bottom`
* Add support for `page-break-before: avoid` and `page-break-after: avoid`
* Bug fixes


Version 0.9
-----------

Released on 2012-06-04.

* Relative, absolute and fixed positioning
* Proper painting order (z-index)
* In PDF: support for internal and external hyperlinks as well as bookmarks.
* Added the ``tree`` parameter to the ``HTML`` class: accepts a parsed lxml
  object.
* Bug fixes, including many crashes.

Bookmarks can be controlled by the ``-weasy-bookmark-level`` and
``-weasy-bookmark-label`` properties, as described in `CSS Generated Content
for Paged Media Module <http://dev.w3.org/csswg/css3-gcpm/#bookmarks>`_.

The default UA stylesheet sets a matching bookmark level on all ``<h1>``
to ``<h6>`` elements.


Version 0.8
-----------

Released on 2012-05-07.

* Switch from cssutils to tinycss_ as the CSS parser.
* Switch to the new cssselect_, almost all level 3 selectors are supported now.
* Support for inline blocks and inline tables
* Automatic table layout (column widths)
* Support for the ``min-width``, ``max-width``, ``min-height`` and
  ``max-height`` properties, except on table-related and page-related boxes.
* Speed improvements on big stylesheets / small documents thanks to tinycss.
* Many bug fixes

.. _tinycss: http://packages.python.org/tinycss/
.. _cssselect: http://packages.python.org/cssselect/


Version 0.7.1
-------------

Released on 2012-03-21.

Change the license from AGPL to BSD.


Version 0.7
-----------

Released on 2012-03-21.

* Support page breaks between table rows
* Support for the ``orphans`` and ``widows`` properties.
* Support for ``page-break-inside: avoid``
* Bug fixes

Only avoiding page breaks before/after an element is still missing.


Version 0.6.1
-------------

Released on 2012-03-01.

Fix a packaging bug. (Remove use_2to3 in setup.py. We use the same
codebase for Python 2 and 3.)


Version 0.6
-----------

Released on 2012-02-29.

* *Backward incompatible*: completely change the Python API.
  See the documentation: http://weasyprint.org/using/#as-a-python-library
* *Backward incompatible*: Proper margin collapsing.
  This changes how blocks are rendered: adjoining margins "collapse"
  (their maximum is used) instead of accumulating.
* Support images in ``embed`` or ``object`` elements.
* Switch to pystacia instead of PIL for raster images
* Add compatibility with CPython 2.6 and 3.2. (Previously only 2.7
  was supported)
* Many bug fixes


Version 0.5
-----------

Released on 2012-02-08.

* Support for the ``overflow`` and ``clip`` properties.
* Support for the ``opacity`` property from CSS3 Colors.
* Support for CSS 2D Transforms. These are prefixed, so you need to use
  ``-weasy-transform`` and ``-weasy-transform-origin``.


Version 0.4
-----------

Released on 2012-02-07.

* Support ``text-align: justify``, ``word-spacing`` and ``letter-spacing``.
* Partial support for CSS3 Paged Media: page size and margin boxes with
  page-based counters.
* All CSS 2.1 border styles
* Fix SVG images with non-pixel units. Requires CairoSVG 0.3
* Support for ``page-break-before`` and ``page-break-after``, except for
  the value ``avoid``.
* Support for the ``background-clip``, ``background-origin`` and
  ``background-size`` from CSS3 (but still with a single background
  per element)
* Support for the ``image-rendering`` from SVG. This one is prefixed,
  use ``-weasy-image-rendering``. It only has an effect on PNG output.


Version 0.3.1
-------------

Released on 2011-12-14.

Compatibility with CairoSVG 0.1.2


Version 0.3
-----------

Released on 2011-12-13.

* **Backward-incompatible change:** the 'size' property is now prefixed (since
  it is in an experimental specification). Use '-weasy-size' instead.
* cssutils 0.9.8 or higher is now required.
* Support SVG images with CairoSVG
* Support generated content: the ``:before`` and ``:after`` pseudo-elements,
  the ``content``, ``quotes`` and ``counter-*`` properties.
* Support ordered lists: all CSS 2.1 values of the ``list-style-type`` property.
* New user-agent stylesheet with HTML 5 elements and automatic quotes for many
  languages. Thanks Peter Moulder!
* Disable cssutils validation warnings, they are redundant with WeasyPrint’s.
* Add ``--version`` to the command-line script.
* Various bug fixes


Version 0.2
-----------

Released on 2011-11-25.

* Support for tables.
* Support the `box-sizing` property from CSS 3 Basic User Interface
* Support all values of vertical-align except top and bottom. They are
  interpreted as text-top and text-bottom.
* Minor bug fixes

Tables have some limitations:
Only the fixed layout and separate border model are supported.
There are also no page break inside tables so a table higher
than a page will overflow.


Version 0.1
-----------

Released on 2011-10-28.

First packaged release. Supports "simple" CSS 2.1 pages: there is no
support for floats, tables, or absolute positioning. Other than that
most of CSS 2.1 is supported, as well as CSS 3 Colors and Selectors.
