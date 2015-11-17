# weektex
研究室用の週報をMarkdownでTexに変換してPDFに出力できるshellscript  
OS X用  

## インストール
### 各種ツールのインストール
- Mactexをインストール  
[Mactexインストールページ](http://tug.org/mactex/mirrorpage.html)  
- GostScriptをインストール  
[GostScriptインストールページ](http://pages.uoregon.edu/koch/)  
- pandocをインストール  

```
$brew install pandoc
```  

brewが入ってない人は下記のリンクを参照してください。  
[MacにHomebrewをインストールする](http://qiita.com/_daisuke/items/d3b2477d15ed2611a058)  

### weektexをcloneする
``` sh
$ git clone git@github.com:kodaitakahashi/weektex.git
```  

### weektexをパスの通った場所にシンボリックリンクを貼る  
header.texのファイルパスの環境変数を定義する  

``` sh
$ export texhead=path/to/header.tex
```   

## 使い方
header.texのtitle,data,authorを変更してください  

```sh
$ weektex 入力するMarkdownファイル
```  

### 例
```sh
$ weektex input.md
```


**これでMacユーザは簡単に週報出せるね!!**
