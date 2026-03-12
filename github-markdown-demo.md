# GitHub Markdown Demo

## Headings

### ATX headings

> [!TIP]
> ATX headings need at least one space between the # characters and the heading text.

```
# h1 heading

## h2 heading

### h3 heading

#### h4 heading

##### h5 heading

###### h6 heading
```

# h1 Heading

## h2 Heading

### h3 Heading

#### h4 Heading

##### h5 Heading

###### h6 Heading

---

### Setext headings

Alternatively, for H1 and H2 (the underlining can be of any length):

```
h1 alternative
=

h2  alternative
------------------------
``` 

h1 alternative
=

h2  alternative
------------------------

---

## Styling text

```
Bold, with **asterisks** or __underscores__.

Italic, with *asterisks* or _underscores_.

Bold with nested italic: **asterisks and _underscores_**.

Bold and italic: ***three asterisks***.

Subscript <sub>text</sub>.

Superscript <sup>text</sup>.

Underlined <ins>text</ins>.

Strikethrough uses two tildes. ~~Scratch this.~~
```

Bold, with **asterisks** or __underscores__.

Italic, with *asterisks* or _underscores_.

Bold with nested italic: **asterisks and _underscores_**.

Bold and italic: ***three asterisks***.

Subscript <sub>text</sub>.

Superscript <sup>text</sup>.

Underlined <ins>text</ins>.

Strikethrough uses two tildes. ~~Scratch this.~~

---

## Quoting text

```
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.

> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.
```

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.

> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.

---

<a name="unique-anchor-name"></a>
## Quoting code and syntax highlighting

### Inline

```
Inline `code` has `` ` `` back-ticks `` ` `` around it.
```

Inline `code` has `` ` `` back-ticks `` ` `` around it.

---

### Block

#### C#

````
```c#
using System.IO.Compression;

#pragma warning disable 414, 3021

namespace MyApplication
{
    [Obsolete("...")]
    class Program : IInterface
    {
        public static List<int> JustDoIt(int count)
        {
            Console.WriteLine($"Hello {Name}!");
            return new List<int>(new int[] { 1, 2, 3 })
        }
    }
}
```
````

```c#
using System.IO.Compression;

#pragma warning disable 414, 3021

namespace MyApplication
{
    [Obsolete("...")]
    class Program : IInterface
    {
        public static List<int> JustDoIt(int count)
        {
            Console.WriteLine($"Hello {Name}!");
            return new List<int>(new int[] { 1, 2, 3 })
        }
    }
}
```

---

#### CSS

````
```css
@font-face {
  font-family: Chunkfive; src: url('Chunkfive.otf');
}

body, .usertext {
  color: #F0F0F0; background: #600;
  font-family: Chunkfive, sans;
}

@import url(print.css);
@media print {
  a[href^=http]::after {
    content: attr(href)
  }
}
```
````

```css
@font-face {
  font-family: Chunkfive; src: url('Chunkfive.otf');
}

body, .usertext {
  color: #F0F0F0; background: #600;
  font-family: Chunkfive, sans;
}

@import url(print.css);
@media print {
  a[href^=http]::after {
    content: attr(href)
  }
}
```

---

#### JavaScript

````
```javascript
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) +
             ` class="${cls}"`;
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }
}

export  $initHighlight;
```
````

```javascript
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) +
             ` class="${cls}"`;
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }
}

export  $initHighlight;
```

---

#### PHP

````
```php
require_once 'Zend/Uri/Http.php';

namespace Location\Web;

interface Factory
{
    static function _factory();
}

abstract class URI extends BaseURI implements Factory
{
    abstract function test();

    public static $st1 = 1;
    const ME = "Yo";
    var $list = NULL;
    private $var;

    /**
     * Returns a URI
     *
     * @return URI
     */
    static public function _factory($stats = array(), $uri = 'http')
    {
        echo __METHOD__;
        $uri = explode(':', $uri, 0b10);
        $schemeSpecific = isset($uri[1]) ? $uri[1] : '';
        $desc = 'Multi
line description';

        // Security check
        if (!ctype_alnum($scheme)) {
            throw new Zend_Uri_Exception('Illegal scheme');
        }

        $this->var = 0 - self::$st;
        $this->list = list(Array("1"=> 2, 2=>self::ME, 3 => \Location\Web\URI::class));

        return [
            'uri'   => $uri,
            'value' => null,
        ];
    }
}

echo URI::ME . URI::$st1;

__halt_compiler () ; datahere
datahere
datahere */
datahere
```
````

```php
require_once 'Zend/Uri/Http.php';

namespace Location\Web;

interface Factory
{
    static function _factory();
}

abstract class URI extends BaseURI implements Factory
{
    abstract function test();

    public static $st1 = 1;
    const ME = "Yo";
    var $list = NULL;
    private $var;

    /**
     * Returns a URI
     *
     * @return URI
     */
    static public function _factory($stats = array(), $uri = 'http')
    {
        echo __METHOD__;
        $uri = explode(':', $uri, 0b10);
        $schemeSpecific = isset($uri[1]) ? $uri[1] : '';
        $desc = 'Multi
line description';

        // Security check
        if (!ctype_alnum($scheme)) {
            throw new Zend_Uri_Exception('Illegal scheme');
        }

        $this->var = 0 - self::$st;
        $this->list = list(Array("1"=> 2, 2=>self::ME, 3 => \Location\Web\URI::class));

        return [
            'uri'   => $uri,
            'value' => null,
        ];
    }
}

echo URI::ME . URI::$st1;

__halt_compiler () ; datahere
datahere
datahere */
datahere
```
___

## Links

```
This is a section link to ['Quoting code and syntax highlighting'](#quoting-code-and-syntax-highlighting).

This is a relative link to ['Quoting code and syntax highlighting'](#unique-anchor-name), because the `unique-anchor-name` anchor is there.

This is a relative reference to a [repository file](../blob/master/LICENSE).

This is a [inline-style link](https://www.google.com) in a sentence.

This is a [inline-style link with title](https://www.google.com "Google's Homepage") in a sentence.

This is a [reference-style link][Arbitrary case-insensitive reference text].

You can use [numbers][1] for reference-style link definitions.

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links: http://www.example.com or <http://www.example.com>.

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com
```

This is a section link to ['Quoting code and syntax highlighting'](#quoting-code-and-syntax-highlighting).

This is a relative link to ['Quoting code and syntax highlighting'](#unique-anchor-name), because the `unique-anchor-name` anchor is there.

This is a relative reference to a [repository file](../blob/master/LICENSE).

This is a [inline-style link](https://www.google.com) in a sentence.

This is a [inline-style link with title](https://www.google.com "Google's Homepage") in a sentence.

This is a [reference-style link][Arbitrary case-insensitive reference text].

You can use [numbers][1] for reference-style link definitions.

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links: http://www.example.com or <http://www.example.com>.

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

---

## Line breaks

```
This example⋅⋅
_(in the actual code, the space symbols are replaced with actual spaces)_⋅⋅
will span three lines.

This example\
will span two lines.

This example<br/>
will span two lines.

This example

will have a blank line separating both lines.
```

This example  
_(in the actual code, the space symbols are replaced with actual spaces)_  
will span three lines.

This example\
will span two lines.

This example<br/>
will span two lines.

This example

will have a blank line separating both lines.

---

## Horizontal rules (AKA thematic breaks)

> [!TIP]
> A line consisting of 0-3 spaces of indentation, followed by a sequence of three or more matching -, \_, or * characters, each followed optionally by any number of spaces or tabs.

> [!TIP]
> Horizontal rules do not need leading or trailing blank lines.

```
___
---
***
   ***
 **  * ** * ** * **
```

___
---
***
   ***
 **  * ** * ** * **

## Images

Here's my logo (hover to see the title text):

> [!TIP]
> You can control avatar's size with the `s` query paramter.

### Inline-style

```
![my logo alt text #1](https://avatars.githubusercontent.com/u/6468893?s=64&v=4  "My Logo Title Text 2")
```

![my logo alt text #1](https://avatars.githubusercontent.com/u/6468893?s=64&v=4  "My Logo Title Text 2")

### Reference-style

```
![my logo alt text #2][logo]

[logo]: https://avatars.githubusercontent.com/u/6468893?s=64&v=4 "My Logo Title Text 2"
```

![my logo alt text #2][logo]

[logo]: https://avatars.githubusercontent.com/u/6468893?s=64&v=4 "My Logo Title Text 2"

### Octocats (HTML needed for size control) 

```
<img width="128" src="https://octodex.github.com/images/minion.png" alt="Minion Octocat Alt Text" title="Minion Octocat Title" />

<img width="128" src="https://octodex.github.com/images/stormtroopocat.jpg" alt="Stormtroopocat Alt Text" title="Stormtroopocat Title" />
```

<img width="128" src="https://octodex.github.com/images/minion.png" alt="Minion Octocat Alt Text" title="Minion Octocat Title" />

<img width="128" src="https://octodex.github.com/images/stormtroopocat.jpg" alt="Stormtroopocat Alt Text" title="Stormtroopocat Title" />

> [!TIP]
> Like links, images also have a footnote style syntax (no size control AFAIK):

```
![Dojocat Alt Text][id]

(with a reference later in the document defining the URL location)

[id]: https://octodex.github.com/images/dojocat.jpg  "Dojocat Title"
```

![Dojocat Alt Text][id]

(with a reference later in the document defining the URL location)

[id]: https://octodex.github.com/images/dojocat.jpg  "Dojocat Title"

---

## Lists

### List example #1 - ordered list with mixed ordered/unordered sub-lists

```
1. Make my changes
    1. Fix bug
    2. Improve formatting
        - Make the headings bigger
2. Push my commits to GitHub
3. Open a pull request
    * Describe my changes
    * Mention all the members of my team
        * Ask for feedback
```

1. Make my changes
    1. Fix bug
    2. Improve formatting
        - Make the headings bigger
2. Push my commits to GitHub
3. Open a pull request
    * Describe my changes
    * Mention all the members of my team
        * Ask for feedback

### List example #2 - ordered list with indented paragraph

```
1. First ordered list item
2. Another item
    * Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
    1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
   *In the actual code, the space symbols are replaced with actual spaces.*⋅⋅
   Note that this line is separate, but within the same paragraph.⋅⋅
   This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.
```

1. First ordered list item
2. Another item
    * Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
    1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.  
   *In the actual code, the space symbols are replaced with actual spaces.*  
   Note that this line is separate, but within the same paragraph.  
   This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.

### List example #3 - simple unordered list with different bullets

```
* Unordered list can use asterisks
- Or minuses
+ Or pluses
```

* Unordered list can use asterisks
- Or minuses
+ Or pluses


### List example #4 - nested unordered lists with different bullets

```
+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces here (see the next tip about the spaces needed):
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!
```

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces here (see the next tip about the spaces needed):
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

> [!TIP]
> Sub-lists are made by indenting by at least the same amount as the preceding list item - the indent length should be at least the same as the length of everything that precedes the text in the preceding list item. Which means 2 for an unordered list (the bullet and its trailing space) or 3 or more for an ordered list (the item index digits and its trailing dot and space)

---

## Task lists

```
- [x] #7
- [ ] Open a pull request
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] List syntax required (any unordered or ordered list supported)
- [x] This is a complete item
- [ ] This is an incomplete item
```

- [x] #7
- [ ] Open a pull request
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] List syntax required (any unordered or ordered list supported)
- [x] This is a complete item
- [ ] This is an incomplete item

---

## Tables

```
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

> [!TIP]
> There must be at least 3 dashes separating each header cell.
> The outer pipes (|) are optional, and you don't need to make the
> raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |

| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |
```

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

> [!TIP]
> There must be at least 3 dashes separating each header cell.
> The outer pipes (|) are optional, and you don't need to make the
> raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |

| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |

---

## Using emojis

```
@octocat :+1: This PR looks great - it's ready to merge! :shipit:
```

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

---

## [Footnotes](https://github.com/markdown-it/markdown-it-footnote)

```
Footnote 1 link[^1].

Footnote 2 link[^2].

Duplicated footnote reference[^2].

[^1]: Footnote **can have markup**⋅⋅
    and multiple paragraphs.

[^2]: Footnote text.
```

Footnote 1 link[^1].

Footnote 2 link[^2].

Duplicated footnote reference[^2].

[^1]: Footnote **can have markup**  
    and multiple paragraphs.

[^2]: Footnote text.

---

## Alerts

```
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
```

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

---

## Escape Markdown formatting characters

You can tell GitHub to ignore (or escape) Markdown formatting by using \ before the Markdown character.

```
Let's rename \*our-new-project\* to \*our-old-project\*.
```

Let's rename \*our-new-project\* to \*our-old-project\*.

---

## Inline HTML

```
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>em</em> and <b>b</b> tags.</dd>
</dl>
```

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>em</em> and <b>b</b> tags.</dd>
</dl>