# ExtendedAbstract
Template for an extended abstract of Master/Bachelor thesis.

## 使い方
### 使う前に
texlive2017以降をインストールしてください．

### コンパイル方法
ディレクトリに移動した後に，
```
latexmk sample.tex
```
をターミナルに入力すると，コンパイルが実行されるはず．

### 自動コンパイル
```
latexmk -pvc sample.tex
```
で変更を確認次第コンパイルが自動で実行されます．

### クリーン
なんかおかしいときは，クリーンしてみましょう．
```
latexmk -c  # 中間ファイルを削除
latexmk -C  # pdfも含めて中間ファイルを削除
```

## 内容物
```
├── .latexmkrc        # o コンパイル設定ファイル
├── README.md         # これ
├── fig               # 画像用フォルダ
│   ├── LaTeX.pdf
│   └── elephant.jpg
├── iml_resume.sty    # o スタイルファイル
├── ipsjunsrt.bst     # o 参考文献の書式ファイル（情報処理学会）
├── sample.pdf        # コンパイルしたpdf見本
├── sample.tex        # o texのテンプレート
├── sample_en.pdf     # コンパイルしたpdf見本
├── sample_en.tex     # o texのテンプレート
├── bibliography.bib  # o 参考文献ファイル（bibファイル）
└── achievement.bib   # o 業績文献ファイル（bibファイル）
```
o から始まるものがおそらく自分のレジュメを書く際に必要なものです．
実行すると他にも色々ファイルができますが，中間ファイルなので最終的には要りません．

## 参考
このテンプレートは，処理系がupLaTeX，文献がbibtexを前提にしています．
TeXには様々なコマンドがありますが，ググると古くなってしまった使い方ばかりが目につくことがあります．
なるべく新しい情報を手に入れるようにしましょう．

以下，このテンプレを作る際に参照したサイトです．

[卒論/修論/博論のためのモダンな LaTeX の書き方](http://webmem.hatenablog.com/entry/how-to-write-a-modern-latex-for-academic-papers)
[現代的 LATEX コードのすすめ](https://prml.main.ist.hokudai.ac.jp/~ryo/contents/textech2016/textech.pdf)
[［改訂新版］upLaTeXを使おう](http://qiita.com/zr_tex8r/items/5c14042078b20edbfb07)
