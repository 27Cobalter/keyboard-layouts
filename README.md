# 自分用にカスタムしたdvorakJP
dvorakjp_custom.scm : WSLのuimで使ってるテーブル
dvorakjp_custom.txt : Mozcで使ってるローマ字テーブル

uimのローマ字テーブルの導入がよくわかってないので`/usr/share/uim/japanese.scm`のja-rk-rule-additionalの中身直接書き換えて使ってる(怒られそう)
```
$ sudo cp /usr/share/uim/japanese.scm /usr/share/uim/japanese.scm.bak
$ sudo nvim -c ":e ++enc=euc-jp" /usr/share/uim/japanese.scm

define ja-rk-rule-additional '( のところで di( して :r ~/path/to/keyboard-layouts/dvorakjp.scm した
```
