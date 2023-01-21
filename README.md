# スライドテンプレート（シンプル設定）

## コンパイルについて

platexを利用します。必要ない場合、`jobname` や `output-directory` は取り除いてください。
```
platex -jobname=output -output-directory=output main.tex
```
上のようにコンパイルした場合は、次のように bibtex を実行してください。
windowsのcmdで実行する場合、パス区切り文字に注意してください。
```
pbibtex output/output.aux
```

相互参照のため、`platex` → `pbibtex` → `platex` → `platex` と実行してください。
`latexmk`など使うと、良い感じにやってくれると思います。

その他、GUIのソフトを使う場合も、`platex`でのコンパイルであれば問題ありません。

出力結果は、[`output/output.pdf`](/output/output.pdf)です。

## ファイルの編集について

[`main.tex`](/main.tex)の`\being{document} ～ \end{document}`の中を編集してください。

数学記号や定理の設定は、[`styles/mysetting.sty`](/styles/mysetting.sty)を編集してください。

## 色設定について

このテンプレートは、`CambridgeUS`というテーマを利用しています。
テーマの設定は、[`styles/mytheme.sty`](/styles/mytheme.sty)で行っています。

ほぼデフォルトで、比較的シンプルな設定になっています。