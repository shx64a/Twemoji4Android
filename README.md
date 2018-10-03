Twemoji4Android
===============

* [Twemoji](https://github.com/twitter/twemoji)を用いたAndroid向けの絵文字フォントを生成するツールです。
* ※「必要なもの」及び「使い方」において、特に注釈等の断りがない場合はUbuntuにおける説明となります。[Mac向けの説明については本家様の記事をご覧下さい。](http://tetsu31415.hatenablog.com/entry/2014/11/22/012845)

# 下準備
必要なパッケージを予めインストールしておきます。
``` terminal
 sudo apt install imagemagick libcairo2 libharfbuzz-bin libpango-1.0-0 librsvg2-bin python-gtk2
```

本家レポジトリからソースを```clone```し、ディレクトリへ```cd```します。
```terminal
 git clone https://github.com/tetsu31415/Twemoji4Android
 cd Twemoji4Android
```

# 使い方
実行するには
``` terminal
make SHELL:=/bin/bash 
```
か、Makefileの1行目に
```
SHELL:=/bin/bash
```
と入力し、

再度makeする場合は一度
``` terminal
make clean
```
を実行してからmakeして下さい[とのことです](https://github.com/tetsu31415/Twemoji4Android/issues/2)。

<!-- ここまで加筆。ここから下は加筆しません。 -->

# Licenses
### Twemoji4Android 
This software is licensed under the MIT License.  
See [LICENSE](LICENSE)

### noto
https://code.google.com/p/noto/  
Copyright 2013 Google, Inc. All Rights Reserved.  
Licensed under the Apache License, Version 2.0.  
See [LICENSE-NOTO](LICENSE-NOTO)

Resources that used in this software:
* nototools/
* color\_emoji/
* third\_party/color\_emoji/

I made the following changes to "add\_glyphs.py" and "emoji\_builder.py":
* The separator for combining characters was changed from "_" to "-".  
* Added glyphs for 0, …, 9, \#, U+20E3.  

### Twemoji
https://github.com/twitter/twemoji  
Copyright 2014 Twitter, Inc and other contributors   
Graphics are licensed under CC-BY 4.0: https://creativecommons.org/licenses/by/4.0/  
See [LICENSE-GRAPHICS](LICENSE-GRAPHICS)  

Resources that used in this software:
* svg/
