# LaTeX
## 概要
LaTeXに関する色々。ほぼ全てのファイルはエンジンにLuaLaTeXを使用している。

無断で使用可能。
## mydocstyle.sty
### 内容
ヘッダ、フッタ、見出し、目次のデザインを提供するパッケージ。その他、一般的なパッケージの読み込み、マクロの定義を含む。ltjsarticleクラスで使用可能。
### 使用方法
目次と見出しのデザインの選択はoptionを指定するだけ。ヘッダとフッタは
```\pagestyle{}```
で指定。
#### 一覧
|見出しoption|目次option|ヘッダ、フッタ(pagestyle)|
|---|---|---|
|sec=normal|toc=normal(default)|normalps|
|sec=1|toc=1|ps=1|
|sec=2| |ps=2|
#### 補足
- toc=normalオプションでは見出しの「目次」の表示位置を変えることができる。`\tableofcontents[pos]`
posはl(left),c(center,default),r(right)から選択する。
- toc=1オプションでは目次の色を変えることができる。`\tableofcontents[color]`
### その他のオプション
1. withlink  
見出しの横に目次ページへのリンクを設置。

## YSdsforrep.sty
### 内容
mydocstyle.styのltjsreportクラス用。
### 使用方法
基本的に前と同じ。
### その他のオプション
1. withlink  
章見出しの横に目次ページへのリンクを設置。節見出しの横には章見出しへのリンク。
2. partialtoc  
章見出しごとに小目次を作成する。
