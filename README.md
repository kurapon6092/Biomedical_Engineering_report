# 生体医工学Ⅰ 課題レポート

## 概要
東京大学の生体医工学Ⅰの課題レポートです。医薬品の探索における熱力学的解析・速度論的解析の重要性について論述しています。

## ファイル構成
- `生体医工学Ⅰ.tex` - メインのLaTeXファイル
- `bio.bib` - 参考文献ファイル
- `alphafold.png` - AlphaFoldで生成したタンパク質構造図
- `README.md` - このファイル

## コンパイル方法
```bash
# 日本語LaTeX環境が必要です
platex -synctex=1 -interaction=nonstopmode 生体医工学Ⅰ.tex
pbibtex 生体医工学Ⅰ
platex -synctex=1 -interaction=nonstopmode 生体医工学Ⅰ.tex
platex -synctex=1 -interaction=nonstopmode 生体医工学Ⅰ.tex
dvipdfmx 生体医工学Ⅰ.dvi
```

## 内容
1. 医薬品の探索について熱力学的解析・速度論的解析が重要な指標になる理由
2. 低分子医薬品・抗体医薬品について医薬品開発を目指す際のアドバンテージおよび懸念点
3. タンパク質の図示（AlphaFold Server使用）