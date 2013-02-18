
Markdown Sample Doc
===================

<h2 id="overview">Overview</h2>

Markdown is intended to be as easy-to-read and easy-to-write as is feasible.

Readability, however, is emphasized above all else. A Markdown-formatted
document should be publishable as-is, as plain text, without looking
like it's been marked up with tags or formatting instructions. While
Markdown's syntax has been influenced by several existing text-to-HTML
filters -- including [Setext] [1], [atx] [2], [Textile] [3], [reStructuredText] [4],
[Grutatext] [5], and [EtText] [6] -- the single biggest source of
inspiration for Markdown's syntax is the format of plain text email.

  [1]: http://docutils.sourceforge.net/mirror/setext.html
  [2]: http://www.aaronsw.com/2002/atx/
  [3]: http://textism.com/tools/textile/
  [4]: http://docutils.sourceforge.net/rst.html
  [5]: http://www.triptico.com/software/grutatxt.html
  [6]: http://ettext.taint.org/doc/


<h3 id="autoescape">Automatic Escaping for Special Characters</h3>

Ampersands in particular are bedeviling for web writers. If you want to
So, if you want to include a copyright symbol in your article, you can write:

&copy;

* * *


This is an H1
=============

This is an H2
-------------


# This is an H1

## This is an H2

###### This is an H6


> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.


Blockquotes can be nested (i.e. a blockquote-in-a-blockquote) by
adding additional levels of `>`:

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

Blockquotes can contain other Markdown elements, including headers, lists,
and code blocks:

> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>     return shell_exec("echo $input | $markdown_script");


<h3 id="list">Lists</h3>

*   Red
*   Green
*   Blue

Ordered lists use numbers followed by periods:

1.  Bird
2.  McHale
3.  Parish

But this:

*   Bird

*   Magic

List items may consist of multiple paragraphs. Each subsequent
paragraph in a list item must be indented by either 4 spaces
or one tab:

1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.


To put a blockquote within a list item, the blockquote's `>`
delimiters need to be indented:

*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

To put a code block within a list item, the code block needs
to be indented *twice* -- 8 spaces or two tabs:

*   A list item with a code block:

        <code goes here>


In other words, a *number-period-space* sequence at the beginning of a
line. To avoid this, you can backslash-escape the period:

1986\. What a great season.



<h3 id="precode">Code Blocks</h3>

Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell


<h3 id="hr">Horizontal Rules</h3>

* * *

***

*****

- - -

---------------------------------------


*single asterisks*

_single underscores_

**double asterisks**

__double underscores__


un*frigging*believable

\*this text is surrounded by literal asterisks\*


<h3 id="code">Code</h3>

Use the `printf()` function.

``There is a literal backtick (`) here.``

`&#8212;` is the decimal-encoded equivalent of `&mdash;`.


* * *


<h2 id="misc">Miscellaneous</h2>

Markdown supports a shortcut style for creating "automatic" links for URLs and email addresses: simply surround the URL or email address with angle brackets. What this means is that if you want to show the actual text of a URL or email address, and also have it be a clickable link, you can do this:

<http://example.com/>
    
<address@example.com>


