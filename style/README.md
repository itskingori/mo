[←](../) Style
==============

> The layout of a document (hence) ... the form of presentation of something.
> ~ [Wikipedia][10]

Git
---

* Use global ignore [(Why?)][2]
* Prefix feature branch names with your initials.
* Write a [good commit message][1].


Formatting
----------

* Break long lines after 80 characters.
* Delete trailing whitespace.
* Don't include spaces after `(`, `[` or before `]`, `)`.
* Don't misspell.
* If you break up an argument list, keep the arguments on their own lines and
  closing parenthesis on its own line.
* If you break up a hash, keep the elements on their own lines and closing curly
  brace on its own line.
* Indent private methods equal to public methods.
* Use 4 space indentation (no tabs).
* Use an empty line between methods.
* Use spaces around operators, after commas, after colons and semicolons, around
  `{` and before `}`.
* Use [Unix-style line endings][3] (`\n`).
* Use uppercase for SQL key words and lowercase for SQL identifiers.


Naming
------

* Avoid abbreviations.
* Avoid types in names (`user_array`).
* Name variables, methods, and classes to reveal intent.
* Treat acronyms as words in names (`XmlHttpRequest` not `XMLHTTPRequest`),
  even if the acronym is the entire name (`class Html` not `class HTML`).


Organization
------------

* Order methods so that caller methods are earlier in the file than the methods
  they call.
* Order methods so that methods are as close as possible to other methods they
  call.


Stylesheets
-----------

### Formatting
* Use the [*LESS*][9] syntax.
* Use hyphens when naming mixins, extends, classes & variables: `span-columns` not `span_columns` or `spanColumns`.
* Use space between property and value: `width: 20px` not `width:20px`.
* Use a blank line above selector that has styles.
* Prefer hex color codes `#000`.
* Use `//` for comment blocks not `/* */`.
* Use a space between selector and `{`.
* Use single quotation marks for attribute selectors and property values.
* Use only lowercase, including colors.
* Don't add a unit specification after `0` values, unless required by a mixin.

### Selectors
* Don't use ID's for style.
* Use meaningful names: `$visual-grid-color` not `$color` or `$vslgrd-clr`.
* Use ID and class names that are as short as possible but as long as necessary.
* Append the prefix `js-` to ID's that are used by Javascript.
* Avoid using the direct descendant selector `>`.
* Avoid nesting more than 4 selectors deep.
* Don't nest more than 6 selectors deep.
* Avoid using the HTML tag in the class name: `section.news` not `section.news-section`.
* Avoid using HTML tags on classes with specific class names like `.featured-articles`.
* Avoid using comma delimited selectors.
* Avoid nesting within a media query.

### Organization
* Use [Normalize][4] as a browser reset.
* Use [HTML5 Boilerplate][7] as your guide to HTML5 best practices.
* Prefer [Foundation][6] by [Zurb][8] as the base layout, then override with custom styles later


File Formats
------------

* Be stored as ASCII text.
* Use ISO-8859-1 or UTF-8 character encoding. The encoding may be declared using
  declare(encoding = 'utf-8'); at the top of the file.
* Be Unix formatted. "Unix formatted" means lines must end only with a line feed
  (LF). Line feeds are represented as ordinal 10, octal 012 and hex 0A. Do not 
  use carriage returns (CR) like Macintosh computers do or the carriage 
  return/line feed combination (CRLF) like Windows computers do.


[1]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
[2]: http://kingori.co/minutae/2013/04/global-ignores/
[3]: http://unix.stackexchange.com/questions/23903/should-i-end-my-text-script-files-with-a-newline
[4]: http://necolas.github.io/normalize.css/
[6]: http://foundation.zurb.com/
[7]: http://html5boilerplate.com/
[8]: http://www.zurb.com/
[9]: http://lesscss.org/#docs
[10]: http://en.wiktionary.org/wiki/format