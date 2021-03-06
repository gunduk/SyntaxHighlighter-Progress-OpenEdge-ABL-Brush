Progress/ABL/OpenEdge SyntaxHighlighter
==========================

What is this?
--------------
This is a brush for [Alex Gorbachev's SyntaxHighlighter][syntaxhighlighterhome], which is a small JavaScript library for general purpose code syntax highlighting.  This brush adds support for the Progress/ABL/OpenEdge programming language (currently, version 10.2A).  Also included is a plugin for the [SyntaxHighlighter Evolved][syntaxhighlighterevolvedhome] plugin by [Viper007Bond][viperhome] for integrating syntax highlighting directly into [Wordpress][wordpresshome].

Why use this?
--------------
Use this brush if you want to highlight Progress/ABL/OpenEdge code on your website or blog.

How to use it
--------------
* For use directly in HTML using the JavaScript SyntaxHighlighter by Alex G., just copy `shBrushABL.js` into the `scripts` directory of SyntaxHighlighters main directory.  Then, simply follow the pattern of the `example.html` file to get the highlighting working (you will basically just wrap your code in `<pre></pre>` tags).
* For Wordpress use, first install the SyntaxHighlighter Evolved plugin and activate it.  Then, copy `shBrushABL.js` and `SyntaxHighlighterEvolved-ABLBrushHook.php` into your `wp-content/plugins/` directory.  The `SyntaxHighlighter Evolved: Progress/ABL/OpenEdge Brush` plugin will now be available within Wordpress Admin, and you can activate it.  To share ABL code directly within your Wordpress posts, simply wrap your code in `[progress][/progress]` or `[abl][/abl]` or `[openedge][/openedge]` tags.  Alternatively, you can use `[code language="abl"][/code]` style tags.

Errata
-------
* The JavaScript was minified using Google's [Closure Compiler][closure].
* Nested comments do not always work correctly, do to an inherent weakness of regular expressions.  There could be workarounds created to handle up to `n` levels of comment nesting, but this works fine for my needs as-is.  I would welcome a patch for this feature!

License
--------
Progress/ABL/OpenEdge SyntaxHighlighter is released under the [LGPLv3][licensesite] license.

[closure]: http://closure-compiler.appspot.com/home
[syntaxhighlighterhome]: http://alexgorbatchev.com/SyntaxHighlighter/
[syntaxhighlighterevolvedhome]: http://wordpress.org/extend/plugins/syntaxhighlighter
[viperhome]: http://www.viper007bond.com
[wordpresshome]: http://wordpress.org
[licensesite]: http://github.com/abevoelker/SyntaxHighlighter-Progress-OpenEdge-ABL-Brush/blob/master/LICENSE
