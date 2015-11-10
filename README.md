#weektex
研究室用の週報をMarkdownでTexに変換してPDFに出力できるshellscript  
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
```shell
$ ./weektex 入力するMarkdownファイル 出力するPDFファイル名
```
###例

```shell
$ chmod u+x ./weektex
$ ./weektex input.md output.pdf
```

 **※実行するディレクトリにheader.texをあることを確認してください。**  

 
**これでMacユーザは簡単に週報出せるね!!**
