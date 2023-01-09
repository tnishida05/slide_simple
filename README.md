# スライドテンプレート（シンプル設定）

## コンパイルについて

lualatexを利用します。必要ない場合、`jobname` や `output-directory` は取り除いてください。
```
lualatex -jobname=output -output-directory=output main.tex
```
上のようにコンパイルした場合は、次のように bibtex を実行してください。
windowsのcmdで実行する場合、パス区切り文字に注意してください。
```
pbibtex output/output.aux
```

相互参照のため、`lualatex` → `pbibtex` → `lualatex` → `lualatex` と実行してください。
`latexmk`など使うと、良い感じにやってくれると思います。

その他、GUIのソフトを使う場合も、`lualatex`でのコンパイルであれば問題ありません。

出力結果は、[`output/output.pdf`](/output/output.pdf)です。

## ファイルの編集について

[`main.tex`](/main.tex)の`\being{document} ～ \end{document}`の中を編集してください。

## 色設定について

このテンプレートは、`CambridgeUS`というテーマを利用しています。

ほぼデフォルトで、シンプルな設定になっています(※当社比)。
ただし、`itemize`など、いくつか設定を変更しています。