#weektex
~~研究室用の週報をMarkdownでTexに変換してPDFに出力できるshellscript~~  
研究室の週報をMarkdownで研究室のフォーマットでTexを出力できるShellscript  
OS X用	
##インストール
1. Maxtexをインストール  
[インストールページ](http://tug.org/mactex/mirrorpage.html)  
1. GostScriptをインストール  
[インストールページ](http://pages.uoregon.edu/koch/)  
1. pandocをインストール  
```
brew install pandoc
```  
brewが入ってない人は下記のリンクを参照してください。  
[MacにHomebrewをインストールする](http://qiita.com/_daisuke/items/d3b2477d15ed2611a058)  
1. cloneする  
```
git clone git@github.com:kodaitakahashi/weektex.git
```  

##使い方
header.texのtitle,data,authorを変更してください  

```sh
$ ./weektex 入力するMarkdownファイル 出力するTexファイル名
```
###例

```sh
$ ./weektex input.md output.tex
```

 **※実行するディレクトリにheader.texをあることを確認してください。**  

 
**これでMacユーザは簡単に週報出せるね!!**
