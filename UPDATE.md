Update process
--------------

Get the latest version of [Normalize.css](http://github.com/necolas/normalize.css) and put it to assets/normalize.css file.

Get the latest version of [Bootstrap](http://getbootstrap.com/). Task if take all styles of base elements without styles for classes (instead table and helpers) and without not really good decisions (IMHO).

Copy print section (@media print) from bootstrap.css to assets/print.css.

Ignore glyphicon styles.

Ignore all styles for classes (instead table, but later about it).

Ignore box-sizing rules for all elements.

Copy html and body styles to assets/basis.css with replacing text color form #333 to #000.

Also copy to assets/basis.css rules for a, img and figure elements (do not remove anchor underline variants comment cheat).

All styles of inputs, selects, fieldsets and other forms components copy to assets/forms_basis.css (do not forget to remove rules for elements with classes).

Styles of other elements copy to assets/content.css but put before every rule class '.content'. Example: `.content hr`.

Add `.content img { max-width: 100%; }` to assets/content.css file.

Save rules for classes '.h1', '.h2', '.h3', '.h4', '.h5', '.h6', '.small', '.mark' and do not insert '.content' class before.

Also save elements with classes 'pull-right' and 'pull-left' - this classes we will save into helpers.

Table styles without classes is boring in bootstrap. Need to compile styles of 'table' and '.table' together and put it to assets/content.css file (with adding '.content' before).

Put to assets/helper.css file usefull universal classes rules:
* .text-left
* .text-right
* .text-center
* .text-justify
* .text-nowrap
* .text-lowercase
* .text-uppercase
* .text-capitalize
* .fade (with modifications)
* .collapse (with modifications)
* .clearfix
* .center-block
* .pull-right
* .pull-left
* .affix
* .hide
* .show
* .invisible
* .text-hide
* .hidden
* .visible-print (with modifications)
* .hidden-print
* maybe something new?

Put to assets/helper.css file `@-ms-viewport` rule.