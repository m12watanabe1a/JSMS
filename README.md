# JSMS

日本材料学会の原稿投稿用のLatexフォーマットです．
オリジナルは[こちら](http://www.jsms.jp/kaishi/k_form.htm)です．

[プレビュー](https://github.com/m12watanabe1a/JSMS/blob/master/jsms.pdf)


## コンパイル
[.latexmk](https://github.com/m12watanabe1a/JSMS/blob/master/.latexmkrc)ファイルを追加したので以下のコマンドでビルドできます．

```bash
$latexmk article.tex
```

### VS Codeのレシピ
VS Codeで[LaTeX Workshop](https://github.com/James-Yu/LaTeX-Workshop)を使用している場合のsettings.jsonの設定は以下を参考にしてください．
```json
    // LaTeX Setup
    "latex-workshop.latex.recipes": [
        {  
            "name": "latexmk",  
            "tools": [  
              "latexmk"  
            ]  
        },
    ],
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
        },
    ],
    "latex-workshop.latex.clean.fileTypes": [
        "*.aux", "*.bbl", "*.blg", "*.idx", "*.ind", "*.lof", "*.lot", "*.out", "*.toc", "*.acn", "*.acr", "*.alg", "*.glg", "*.glo", "*.gls", "*.ist", "*.fls", "*.log", "*.fdb_latexmk", "*.synctex.gz",
        "_minted*", "*.nav", "*.snm", "*.vrb",
        "*.run.xml","*.dvi","*.bcf"
    ],
    "latex-workshop.view.pdf.viewer": "tab",
    "latex-workshop.latex.autoClean.run": "onFailed",
```
