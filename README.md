MadokoCJK
=========

CJK Template for [Madoko](https://madoko.net), a super powerful markdown processor (and a dialect).

Usage
-----

Just put the template files in the `styles` subdir or just the root dir of your document. Include it like:

```Markdown
<!-- Normal Metadata Defs -->
Title    : 一个例子
Author   : 赵明毅
<!-- ... -->

<!-- MadokoCJK Defs -->
<!--
CJKLang  : zh-Hans-CN <!-- An ISO-636 name of one of the supported languages -->
<!-- For now, use these unfortunate boolean switches: -->
CJK_zh   : True       <!-- CJK_zh{,_CN,_TW}, CJK_ja, CJK_kr -->
CJKHanzi : True       <!-- If we should use hanzi.css. Boolean; True/False -->
CJKXeCJK : False      <!-- If we should use XeCJK font list instead of ctex -->
[INCLUDE=styles/madokocjk.mdk]
```

Support Roadmap
---------------

- Madoko-level Support
  - [ ] Prelude babels (zh_CN: incoming)
- HTML Support
  - [ ] `.madoko { html-lang: LANG; }` support (very easy)
  - [ ] [hanzi.css](https://css.hanzi.co/) integration
- XeLaTeX Support
  - [ ] `\usepackage[UTF8]{ctex}` (zh_\*, hyper easy)
  - [ ] XeCJK font presets for offical madoko.net
