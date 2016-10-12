.. role:: small

Inline Markup
-------------

*emphasis*,  **strong emphasis**, `interpreted text`, ``inline literal``.

.. code-block:: rst

    *emphasis*,  **strong emphasis**, `interpreted text`, ``inline literal``.


References and Links
--------------------

ref_, :ref:`target`, `link <http://example.com/>`_, :doc:`rst-cheatsheet`

.. code-block:: rst

    reference_, :ref:`reference`, `link <http://example.com/>`_, :doc:`rst-cheatsheet`


.. _target:

Targets
-------

.. _ref: http://example.com

.. code-block:: rst

    .. _reference: http://example.com

Lists
-----

- item list
- no extra space before dash

  - add blank line above
    
    .. code-block:: php
    
        echo 2+2;

  - keep alignment
    and can use more lines

.. code-block:: rst

    - item
    - list

      - add blank line above
        
        .. code-block:: php
        
            echo 2+2;

      - keep alignment
        and you can use more lines

Numeric Lists
`````````````

1. Numeric List
#. is auto-numbered

   #. use line above and below

    a. or single space in alignment
    #. various numbering options

   #. sometimes '#' fails
   #. so use numbers
#. here '#' works though.

.. code-block:: rst

    1. Numeric List
    #. is auto-numbered

       #. use line above

        a. or single space in alignment
        #. various numbering options

       #. sometimes '#' fails
       #. so use numbers
    #. here '#' works though.

Definition Lists
````````````````

definition list
    here is example::

        echo 2+2;
inline code
    can be also used.

    .. code-block:: json

        {"A":123}

.. code-block:: rst

    definition list
        here is example::

            echo 2+2;
    inline code
        can be also used.

        .. code-block:: json

            {"A":123}


Option Lists
````````````

-a           option list start with '-' and a line
--arguments  will have a special treatment
/dos         for application arguments

.. code-block:: rst

    -a           option list start with '-' and a line
    --arguments  will have a special treatment
    /dos         for application arguments


.. raw:: pdf

   Spacer 0 4

Section Structure
-----------------

+----------------------------------------------------------+--------------------------------------------------------+
| ::                                                       |                                                        |
|                                                          |   .. class:: faketitle                                 |
|    Title                                                 |                                                        |
|    =====                                                 |   Title                                                |
|                                                          |                                                        |
|    Titles are underlined (or over- and underlined) with  |   Titles are underlined (or over- and underlined) with |
|    a nonalphanumeric character at least as long as the   |   a nonalphanumeric character at least as long as the  |
|    text.                                                 |   text.                                                |
|                                                          |                                                        |
|    A lone top-level section is lifted up to be the       |   A lone top-level section is lifted up to be the      |
|    document's title                                      |   document's title                                     |
|                                                          |                                                        |
+----------------------------------------------------------+--------------------------------------------------------+

Blocks
------

+---------------------------------------------------------------+------------------------------------------------------+
| ::                                                            |                                                      |
|                                                               |                                                      |
|    This is a paragraph.                                       | This is a paragraph.                                 |
|                                                               |                                                      |
|    Paragraphs line up at their left edges, and are            | Paragraphs line up at their left                     |
|    normally separated by blank lines.                         | edges, and are normally separated                    |
|                                                               | by blank lines.                                      |
+---------------------------------------------------------------+------------------------------------------------------+
| ::                                                            |                                                      |
|                                                               |                                                      |
|    A paragraph containing only two colons indicates           |    A paragraph containing only two colons            |
|    the following indented or quoted text is a literal         |    indicates that the following indented             |
|    block or quoted text is a literal block.                   |    or quoted text is a literal block.                |
|                                                               |                                                      |
|    ::                                                         |    ::                                                |
|                                                               |                                                      |
|      Whitespace, newlines, blank lines, and  all kinds of     |      Whitespace, newlines, blank lines, and          |
|      markup (like *this* or \this) is preserved here.         |      all kinds of markup (like *this* or             |
|                                                               |      \this) is preserved by literal blocks.          |
|    You can also tack the ``::`` at the end of a               |                                                      |
|    paragraph::                                                |    You can also tack the ``::`` at the end of a      |
|                                                               |    paragraph::                                       |
|       It's very convenient to use this form.                  |                                                      |
|                                                               |      It's very convenient to use this form.          |
|    Per-line quoting can also be used for unindented           |                                                      |
|    blocks::                                                   |    Per-line quoting can also be used for             |
|                                                               |    unindented blocks::                               |
|    > Useful for quotes from email and                         |                                                      |
|    > for Haskell literate programming.                        |    > Useful for quotes from email and                |
|                                                               |    > for Haskell literate programming.               |
+---------------------------------------------------------------+------------------------------------------------------+
| ::                                                            |                                                      |
|                                                               |                                                      |
|    | Line blocks are useful for addresses,                    |    | Line blocks are useful for addresses,           |
|    | verse, and adornment-free lists.                         |    | verse, and adornment-free lists.                |
|    |                                                          |    |                                                 |
|    | Each new line begins with a                              |    | Each new line begins with a                     |
|    | vertical bar ("|").                                      |    | vertical bar ("|").                             |
|    |     Line breaks and initial indents                      |    |     Line breaks and initial indents             |
|    |     are preserved.                                       |    |     are preserved.                              |
|    | Continuation lines are wrapped                           |    | Continuation lines are wrapped                  |
|      portions of long lines; they begin                       |      portions of long lines; they begin              |
|      with spaces in place of vertical bars.                   |      with spaces in place of vertical bars.          |
+---------------------------------------------------------------+------------------------------------------------------+
| ::                                                            |                                                      |
|                                                               |                                                      |
|   Block quotes are just:                                      |   Block quotes are just:                             |
|                                                               |                                                      |
|       Indented paragraphs,                                    |       Indented paragraphs,                           |
|                                                               |                                                      |
|           and they may nest.                                  |           and they may nest.                         |
+---------------------------------------------------------------+------------------------------------------------------+
| ::                                                            |                                                      |
|                                                               |                                                      |
|   Doctest blocks are interactive                              |   Doctest blocks are interactive                     |
|   Python sessions. They begin with                            |   Python sessions. They begin with                   |
|   "``>>>``" and end with a blank line.                        |   "``>>>``" and end with a blank line.               |
|                                                               |                                                      |
|   >>> print "This is a doctest block."                        |   >>> print "This is a doctest block."               |
|   This is a doctest block.                                    |   This is a doctest block.                           |
+---------------------------------------------------------------+------------------------------------------------------+

.. raw:: pdf

   PageBreak

Tables
------

There are two syntaxes for tables in reStructuredText. Grid tables are complete but cumbersome to create. Simple
tables are easy to create but limited (no row spans, etc.).

+------------+------------+-----------+
| Header 1   | Header 2   | Header 3  |
+============+============+===========+
| body row 1 | column 2   | column 3  |
+------------+------------+-----------+
| body row 2 | Cells may span columns.|
+------------+------------+-----------+
| body row 3 | Cells may  | - Cells   |
+------------+ span rows. | - contain |
| body row 4 |            | - blocks. |
+------------+------------+-----------+

=====  =====  ======
   Inputs     Output
------------  ------
  A      B    A or B
=====  =====  ======
False  False  False 
True   False  True  
False  True   True  
True   True   True  
=====  =====  ======

------------------------------------------------------------+------------------------------------------------------+

Explicit Markup
---------------

Explicit markup blocks are used for constructs which float (footnotes), have no direct paper-document representation
(hyperlink targets, comments), or require specialized processing (directives).
They all begin with two periods and whitespace, the "explicit markup start".

+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   Footnote references, like [5]_.                             |   Footnote references, like [5]_.                           |
|   Note that footnotes may get                                 |   Note that footnotes may get                               |
|   rearranged, e.g., to the bottom of                          |   rearranged, e.g., to the bottom of                        |
|   the "page".                                                 |   the "page".                                               |
|                                                               |                                                             |
|   .. [5] A numerical footnote. Note                           |   .. [5] A numerical footnote. Note                         |
|      there's no colon after the ``]``.                        |      there's no colon after the ``]``.                      |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   Autonumbered footnotes are                                  |   Autonumbered footnotes are                                |
|   possible, like using [#]_ and [#]_.                         |   possible, like using [#]_ and [#]_.                       |
|                                                               |                                                             |
|   .. [#] This is the first one.                               |   .. [#] This is the first one.                             |
|   .. [#] This is the second one.                              |   .. [#] This is the second one.                            |
|                                                               |                                                             |
|   They may be assigned 'autonumber                            |   They may be assigned 'autonumber                          |
|   labels' - for instance,                                     |   labels' - for instance,                                   |
|   [#fourth]_ and [#third]_.                                   |   [#fourth]_ and [#third]_.                                 |
|                                                               |                                                             |
|   .. [#third] a.k.a. third_                                   |   .. [#third] a.k.a. third_                                 |
|                                                               |                                                             |
|   .. [#fourth] a.k.a. fourth_                                 |   .. [#fourth] a.k.a. fourth_                               |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   Auto-symbol footnotes are also                              |   Auto-symbol footnotes are also                            |
|   possible, like this: [*]_ and [*]_.                         |   possible, like this: [*]_ and [*]_.                       |
|                                                               |                                                             |
|   .. [*] This is the first one.                               |   .. [*] This is the first one.                             |
|   .. [*] This is the second one.                              |   .. [*] This is the second one.                            |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   Citation references, like [CIT2002]_.                       |   Citation references, like [CIT2002]_.                     |
|   Note that citations may get                                 |   Note that citations may get                               |
|   rearranged, e.g., to the bottom of                          |   rearranged, e.g., to the bottom of                        |
|   the "page".                                                 |   the "page".                                               |
|                                                               |                                                             |
|   .. [CIT2002] A citation                                     |   .. [CIT2002] A citation                                   |
|      (as often used in journals).                             |      (as often used in journals).                           |
|                                                               |                                                             |
|   Citation labels contain alphanumerics,                      |   Citation labels contain alphanumerics,                    |
|   underlines, hyphens and fullstops.                          |   underlines, hyphens and fullstops.                        |
|   Case is not significant.                                    |   Case is not significant.                                  |
|                                                               |                                                             |
|   Given a citation like [this]_, one                          |   Given a citation like [this]_, one                        |
|   can also refer to it like this_.                            |   can also refer to it like this_.                          |
|                                                               |                                                             |
|   .. [this] here.                                             |   .. [this] here.                                           |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   External hyperlinks, like Python_.                          |   External hyperlinks, like Python_.                        |
|                                                               |                                                             |
|   .. _Python: http://www.python.org/                          |   .. _Python: http://www.python.org/                        |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   External hyperlinks, like `Python                           |   External hyperlinks, like `Python                         |
|   <http://www.python.org/>`_.                                 |   <http://www.python.org/>`_.                               |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   Internal crossreferences, like example_.                    |   Internal crossreferences, like example_.                  |
|                                                               |                                                             |
|   .. _example:                                                |   .. _example:                                              |
|                                                               |                                                             |
|   This is an example crossreference target.                   |   This is an example crossreference target.                 |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   Python_ is `my favourite                                    |   Python_ is `my favourite                                  |
|   programming language`__.                                    |   programming language`__.                                  |
|                                                               |                                                             |
|   .. _Python: http://www.python.org/                          |   .. _Python: http://www.python.org/                        |
|                                                               |                                                             |
|   __ Python_                                                  |   __ Python_                                                |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |   .. _titles are targets, too:                              |
|                                                               |   .. class:: faketitle                                      |
|   Titles are targets, too                                     |                                                             |
|   =======================                                     |   Titles are targets, too                                   |
|                                                               |                                                             |
|   Implict references, like `Titles are targets, too`_.        |   Implict references, like                                  |
|                                                               |   `Titles are targets, too`_.                               |
+---------------------------------------------------------------+-------------------------------------------------------------+
|                                                                                                                             |
|Directives are a general-purpose extension mechanism, a way of adding support for new constructs without adding              |
|new syntax. For a description of all standard directives, see reStructuredText Directives (http://is.gd/2Ecqh).              |
|                                                                                                                             |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   For instance:                                               |   For instance:                                             |
|                                                               |                                                             |
|   .. image:: magnetic-balls.jpg                               |   .. image:: magnetic-balls.jpg                             |
|      :width: 40pt                                             |      :width: 40pt                                           |
|                                                               |                                                             |
+---------------------------------------------------------------+-------------------------------------------------------------+
|                                                                                                                             |
|                                                                                                                             |
| Substitutions are like inline directives, allowing graphics and arbitrary constructs within text.                           |
|                                                                                                                             |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   The |biohazard| symbol must be used on containers used to   |   The |biohazard| symbol must be used on containers used to |
|   dispose of medical waste.                                   |   dispose of medical waste.                                 |
|                                                               |                                                             |
|   .. |biohazard| image:: biohazard.png                        |   .. |biohazard| image:: biohazard.png                      |
|      :align: middle                                           |      :align: middle                                         |
|      :width: 12                                               |      :width: 12                                             |
+---------------------------------------------------------------+-------------------------------------------------------------+
|                                                                                                                             |
| Any text which begins with an explicit markup start but doesn't use the syntax of any of the constructs above, is a comment.|
|                                                                                                                             |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   .. This text will not be shown                              |   .. This text will not be shown                            |
|      (but, for instance, in HTML might be                     |      (but, for instance, in HTML might be                   |
|      rendered as an HTML comment)                             |      rendered as an HTML comment)                           |
+---------------------------------------------------------------+-------------------------------------------------------------+
| ::                                                            |                                                             |
|                                                               |                                                             |
|   An "empty comment" does not                                 |   An "empty comment" does not                               |
|   consume following blocks.                                   |   consume following blocks.                                 |
|   (An empty comment is ".." with                              |   (An empty comment is ".." with                            |
|   blank lines before and after.)                              |   blank lines before and after.)                            |
|                                                               |                                                             |
|   ..                                                          |   ..                                                        |
|                                                               |                                                             |
|           So this block is not "lost",                        |           So this block is not "lost",                      |
|           despite its indentation.                            |           despite its indentation.                          |
+---------------------------------------------------------------+-------------------------------------------------------------+

Credits
-------

.. class:: tablacreditos

+---------------------------------------+-------------------------------------------------------+
| CP Font from LiquiType:               | http://www.liquitype.com/workshop/type_design/cp-mono |
+---------------------------------------+-------------------------------------------------------+
| Magnetic Balls V2 image by fdecomite: | http://www.flickr.com/photos/fdecomite/2926556794/    |
+---------------------------------------+-------------------------------------------------------+
| Sponsored by Net Managers             | http://www.netmanagers.com.ar                         |
+---------------------------------------+-------------------------------------------------------+
| Typeset using rst2pdf                 | http://rst2pdf.googlecode.com                         |
+---------------------------------------+-------------------------------------------------------+


.. footer::

    .. class:: tablapie

    +-------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------+----------------------------------+-----------------------------------+
    | |copy| :small:`2009 Roberto Alsina <ralsina@netmanagers.com.ar>  /  Creative Commons Attribution-Noncommercial-Share Alike 2.5 Argentina License`     | |attrib| :small:`Based on quickref.txt from docutils`               | |noncomm| :small:`Non-Commercial`| |sharealike| :small:`Share Alike` |
    +-------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------+----------------------------------+-----------------------------------+

.. |attrib| image:: attrib.png
   :width: 8pt
   :align: middle

.. |noncomm| image:: noncomm.png
   :width: 8pt
   :align: middle

.. |sharealike| image:: sharealike.png
   :width: 8pt
   :align: middle

.. |copy|   unicode:: U+000A9
