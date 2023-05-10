# WSLでlatexを使う

## setup

https://zenn.dev/umi_mori/books/72d30926afbc24/viewer/c4f8a3

- install latex workshop expansion
- setting.json
```
    // ===== Latex =====
    // 使用パッケージのコマンドや環境の補完を有効にする
    "latex-workshop.intellisense.package.enabled": true,
    "latex-workshop.latex.outDir": "latex-output",

    // ビルドのレシピ
    "latex-workshop.latex.recipes": [
        {
            "name": "latexmk",
            "tools": [
                "latexmk"
            ]
        },
    ],

    // ビルドのレシピに使われるパーツ
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-silent",
                "-outdir=%OUTDIR%",
                "%DOC%"
            ],
        },
    ],
    "latex-workshop.view.pdf.viewer": "tab",
```
