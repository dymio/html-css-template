Update process
--------------

1. Get the latest version of
    [Normalize.css](http://github.com/necolas/normalize.css)
    and put it to assets/normalize.css file.

2. Get the latest version of [Bootstrap](http://getbootstrap.com/) css file.
    Get all styles of elements without classes (instead of table and clearfix).
    Skip not good decisions (like 'box-sizing: border-box' for all, IMHO).

3. Media print section (@media print) put to print.css file.

4. Ignore box-sizing rules for `*, *:before, *:after` elements.

5. Update all commont styles in basis.css file: for html, body, a, figure, img
    tags, forms styles, '@-ms-viewport' rule etc.

6. Update styles of content elements in content.css. Don't forget to add
    '.content' selector before added css rule.
    Content elements are elements which user can add by wysiwyg editor.
    Paragraphs, headers, hr, lists, tables etc.

    6.1. Table styles without classes is boring in Bootstrap. Compile styles
        of table element and '.table' class together.

    6.2. Do not remove `.content img { max-width: 100%; }` from content.css.

7. Update [readme file](README.md): last update date and component versions.

8. Update last update in [humans txt](humans.txt) file;
