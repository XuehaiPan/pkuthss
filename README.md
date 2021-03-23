**iofu728-pkuthss**: Modified version of `LaTeX` Peking University thesis template base on [CasperVector/pkuthss](https://github.com/CasperVector/pkuthss) v1.9.0

[**Overleaf** Version](https://www.overleaf.com/latex/templates/2021-peking-university-master-thesis-template-iofu728-pkuthss/rwfvbkpzydpf) is public, welcome to use!

## Overview

To use pkuthss in the overleaf platform, and to support some customization requirements in writing processing, I redevelop the template of pkuthss.

**Modified details:**

- Style Part:

  - Fixed the styles of table of contents(chapter);
  - Fixed `KEY WORDS`, `Title` in the cover -> remove the setting of `bold`;
  - Fixed Font Size / Font in the cover, like title and keys;
  - Hind hreflink;

- Functional Part:
  - Support library inspection requirements;
  - Supported Overleaf online mode;
  - Support denotation table;
  - Support subfigure \ref, footnote in table;
  - Supported scanned pdf insert(origin and copy pages);
  - Add fontset mode, change bfseries -> AutoFakeBold in windows;
  - Simplify user settings in blind mode;

## Quick Start

_Requirements_

- TextLive(In mac, you can use MacTex)

```bash
> cd tex && make all
> cd ../doc/example && latexmk
```

## Notes and Acknowledgments

This code base is built on top of [CasperVector/pkuthss](https://github.com/CasperVector/pkuthss).

The following files have been changed

- .gitignore
- README.md
- tex/pkuthss.cls
- tex/pkuthss-\*.def
- tex/Makefile
- doc/example/chap/\*
- doc/example/latexmkrc
- doc/example/thesis.bib
- doc/example/thesis.tex

## ToDo Lists

- [x] Check Table and Fig Setting.
- [x] Support Overleaf.
- [x] Fix table of contents.
- [x] Support insert pdf (copy and origin pages).
- [x] Adaptive pkuthss v1.9.0.

## Change Log

See [CHANGELOG.md](CHANGELOG.md) for the detailed changes in each release.

## QA in chinese

1. Q: 原创页使用这种方式生成得到的文件与 Mac 端字体不同。

A: 门户生成的 PDF 文件将字体信息写入文件，导致在 Mac 端呈现字体效果不同(Mac 端显示的是华文字体，而 Windows 端显示的是中易字体)。
请务必在 Windows 系统下进行打印，或者使用本包生成文件进行打印。

## Lincense

This repository following [LaTeX Project Public License](http://www.latex-project.org/lppl.txt) and [Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.en).
