[トップページに戻る](README.md)

# [FTKR_ExEquipSlot](FTKR_ExEquipSlot.js) プラグイン

同じ装備タイプの装備を２つ以上装備できるようにするプラグインです。

ダウンロード: [FTKR_ExEquipSlot.js](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExEquipSlot.js)

## 目次

以下の項目の順でプラグインの使い方を説明します。
1. [概要](#概要)
* [プラグインの更新履歴](#プラグインの更新履歴)
* [ライセンス](#ライセンス)

## 概要

同じ装備タイプの装備を２つ以上装備できるようにします。

## 設定方法
複数装備させたい装備タイプを、データベースの装備タイプに同じ名前で装備させたい数だけ設定してください。

設定した装備タイプの装備は、同じ名前の装備スロットであれば
どこにでも装備可能になります。

### ＜注意＞
装備タイプ「武器」を増やすと、スロットタイプ「二刀流」と同等の効果が発生します。

## 同じ武器・防具を複数装備させる場合
プラグインパラメータ`<Enable Equip Same Items>`で同じ武器・防具を複数装備できるか設定できます。

「装備できる」に設定した場合は、同じ装備を２つ以上装備できます。
「装備できない」に設定した場合は、同じ装備は１つしか装備できません。

ただし、以下のタグをメモ欄に記載すると、プラグインパラメータの設定を無視するようになります。

`<EES_複数装備可>`

このタグがある装備は、`<Enable Equip Same Items>`を「装備できない」に設定していても、複数装備可能になります。

`<EES_複数装備不可>`

このタグがある装備は、`<Enable Equip Same Items>`を「装備できる」に設定していても、１つしか装備できません。


## 同じ武器タイプ、防具タイプを複数装備させない場合
基本的に同じ武器タイプ・防具タイプは、何個でも装備可能になります。

ただし、以下のプラグインパラメータに数値を入力するとそのIDの武器タイプや防具タイプは、１つしか装備できません。

`<Disabled Equip Same Wtypes>`

このパラメータに入力した武器タイプIDは、１つしか装備できません。
複数のIDを入力する場合は、カンマ(,)で分けてください。
また、二つのID同士をハイフン(-)で繋げた場合は、その間のすべてのIDを登録します。

`<Disabled Equip Same Atypes>`

このパラメータに入力した防具タイプIDは、１つしか装備できません。
複数のIDを入力する場合は、カンマ(,)で分けてください。
また、二つのID同士をハイフン(-)で繋げた場合は、その間のすべてのIDを登録します。

### 入力例
```
1, 4, 5, 10-15
```
この場合、ID 1, 4, 10, 11, 12, 13, 14, 15が該当します。

[目次に戻る](#目次)

# プラグインの更新履歴

| バージョン | 公開日 | 更新内容 |
| --- | --- | --- |
| [ver1.2.0](FTKR_ExEquipSlot.js) | 2018/12/20 | 同じ武器タイプ防具タイプを複数装備させない機能を追加 |
| ver1.1.0 | 2017/12/17 | 同じ装備を２つ以上装備できるか設定する機能を追加 |
| ver1.0.0 | 2017/06/30 | 新規作成 |

# ライセンス

本プラグインはMITライセンスのもとで公開しています。

[The MIT License (MIT)](https://opensource.org/licenses/mit-license.php)

#
[目次に戻る](#目次)

[トップページに戻る](README.md)