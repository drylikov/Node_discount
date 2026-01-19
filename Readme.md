
# Markdown.js

  node bindings for the C "discount" markdown implementation by David Parsons.
  
## Installation

    $ npm install discount
  
## Usage

    var md = require('discount');
    md.parse('markdown is *awesome*')
    // => '<p>markdown is <em>awesome</em></p>'

### Flags

    md.parse('[links](http://github.com/) are *not* allowed here', md.flags.noLinks)
    // => '<p>[links](http://github.com/) are <em>not</em> allowed here</p>'

All [Discount flags](http://www.pell.portland.or.us/~orc/Code/discount/#flags) are supported:
`noLinks`, `noImage`, `noPants`, `noHTML`, `strict`, `tagText`, `noExt`, `cdata`, `noSuperscript`, `noRelaxed`, `noTables`, `noStrikethrough`, `toc`, `md1Compat`, `autolink`, `safelink`, `noHeader`, `tabStop`, `noDivQuote`, `noAlphaList`, `noDlist` and `extraFootnote`.



