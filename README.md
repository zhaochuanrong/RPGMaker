# RPGツクールMV プラグイン

プラグインは逐次追加更新を行っています。最新情報は、[更新情報](#更新情報)を確認してください。

# 目次

1. [ステータス](#ステータス)
1. [変数_スイッチ](#変数_スイッチ)
1. [ウィンドウ](#ウィンドウ)
1. [メッセージ](#メッセージ)
1. [アイテム_スキル仕様拡張](#アイテム_スキル仕様拡張)
1. [スキル](#スキル)
1. [アイテム](#アイテム)
1. [ステート](#ステート)
1. [敵グループ](#敵グループ)
1. [バトル](#バトル)
1. [イベント](#イベント)
1. [マップ](#マップ)
1. [セーブ](#セーブ)
1. [ミニゲーム](#ミニゲーム)
1. [デバッグ](#デバッグ)
1. [その他備忘録](#その他備忘録)
1. [試作品置き場](#試作品置き場)
1. [更新情報](#更新情報)


# ステータス

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_AddOriginalParameters](FTKR_AddOriginalParameters.js) | [あり](FTKR_AddOriginalParameters.ja.md) | [v1.1.6](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_AddOriginalParameters.js) | 2017/11/05 |オリジナルパラメータを追加する |
| [FTKR_SearchPartyParam](FTKR_SearchPartyParam.js) | [あり](FTKR_SearchPartyParam.ja.md) | [v1.0.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SearchPartyParam.js) | 2017/04/14 | パーティー内のパラメータに関するスクリプトを実装する |
| [FTKR_ExSvMotion](FTKR_ExSvMotion.js) | [仮版](FTKR_ExSvMotion.ja.md) | [v1.2.5](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExSvMotion.js) | 2017/08/24 | SVキャラのモーションを拡張する |
| [FTKR_FacialImageDifference](FTKR_FacialImageDifference.js) | [仮版](FTKR_FacialImageDifference.ja.md) | [v1.1.7](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_FacialImageDifference.js) | 2017/12/02 | アクターの状態によって顔画像を変える<br>顔画像にアニメーションを表示する |
| [FTKR_FacialImageDifference2](FTKR_FacialImageDifference2.js) | なし | [v2.0.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_FacialImageDifference2.js) | 2017/12/16 | アクターの状態によって顔画像を変える<br>FTKR_FacialImageDifference.jsと組み合わせて使用できません |
| [FTKR_ExTraitSetting](FTKR_ExTraitSetting.js) | なし | [v1.0.4](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExTraitSetting.js) | 2018/02/17 | 装備やステート等の特徴を詳細に設定できる |

## ステータス表示の変更

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) | [あり](FTKR_CustomSimpleActorStatus.ja.md) | [v2.6.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CustomSimpleActorStatus.js) | 2018/01/07 | ステータス表示を変更する 本体プラグイン |
| [FTKR_CSS_MenuStatus](FTKR_CSS_MenuStatus.js) | [あり](FTKR_CSS_MenuStatus.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_MenuStatus.js) | 2017/11/18 | メニュー画面のステータス表示を変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |
| [FTKR_CSS_BattleStatus](FTKR_CSS_BattleStatus.js) | [あり](FTKR_CSS_BattleStatus.ja.md) | [v1.3.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_BattleStatus.js) | 2017/11/18 | バトル画面のステータス表示を変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |
| [FTKR_CSS_DetailedStatus](FTKR_CSS_DetailedStatus.js) | [あり](FTKR_CSS_DetailedStatus.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_DetailedStatus.js) | 2017/11/18 | ステータス画面のステータス表示を変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |
| [FTKR_CSS_SkillStatus](FTKR_CSS_SkillStatus.js) | [あり](FTKR_CSS_SkillStatus.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_SkillStatus.js) | 2017/11/18 | スキル画面のステータス表示を変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |
| [FTKR_CSS_EquipStatus](FTKR_CSS_EquipStatus.js) | [仮版](FTKR_CSS_EquipStatus.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_EquipStatus.js) | 2017/11/18 | 装備画面のステータス表示を変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |
| [FTKR_CSS_ShopStatus](FTKR_CSS_ShopStatus.js) | [仮版](FTKR_CSS_ShopStatus.ja.md) | [v1.2.2](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_ShopStatus.js) | 2017/12/02 | ショップ画面のステータス表示を変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |
| [FTKR_CSS_CustomizeBattleResults](FTKR_CSS_CustomizeBattleResults.js) | [仮版](FTKR_CSS_CustomizeBattleResults.ja.md) | [v1.4.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CSS_CustomizeBattleResults.js) | 2018/01/12 | バトル終了時に戦闘結果を表示する <br> ＜以下のプラグインが必要＞ <br> [FTKR_CustomSimpleActorStatus](FTKR_CustomSimpleActorStatus.js) |

FTKR_CSS_GDMはFTKR_CustomSimpleActorStatusに統合しました

[目次に戻る](#目次)

# 変数_スイッチ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ItemSelfVariables](FTKR_ItemSelfVariables.js) | [あり](FTKR_ItemSelfVariables.ja.md) | [v1.2.2](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemSelfVariables.js) | 2018/01/08 | アイテム、スキル、アクター、エネミーにセルフ変数を追加する |
| [FTKR_ExVariablesChange](FTKR_ExVariablesChange.js) | [仮版](FTKR_ExVariablesChange.ja.md) | [v1.2.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExVariablesChange.js) | 2017/08/24 | 変数の操作を拡張するプラグイン |
| [FTKR_EventSelfSwOperation](FTKR_EventSelfSwOperation.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_EventSelfSwOperation.js) | 2017/04/25 | イベントのセルフスイッチを操作するプラグイン |

[目次に戻る](#目次)

# ウィンドウ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_DisplayCommandFrame](FTKR_DisplayCommandFrame.js) | [仮版](FTKR_DisplayCommandFrame.ja.md) | [v1.2.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_DisplayCommandFrame.js) | 2017/11/26 | コマンドに枠を付ける |
| [FTKR_OriginalSceneWindow](FTKR_OriginalSceneWindow.js) | [仮版](FTKR_OriginalSceneWindow.ja.md) | [v1.5.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_OriginalSceneWindow.js) | 2018/02/15 | オリジナルのシーンおよびウィンドウを作成する |
| [FTKR_SceneBackImages](FTKR_SceneBackImages.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SceneBackImages.js) | 2018/02/24 | メニュー画面やショップ画面などに変数で切替可能な背景画像を設定する |
| [FTKR_InterlockMouseAndWindow](FTKR_InterlockMouseAndWindow.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_InterlockMouseAndWindow.js) | 2018/02/25 | マウスポインタとウィンドウのカーソルを連動させる |

[目次に戻る](#目次)

# メッセージ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ExEscapeCharacters](FTKR_ExEscapeCharacters.js) | [仮版](FTKR_ExEscapeCharacters.ja.md) | [v1.0.2](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExEscapeCharacters.js) | 2017/03/28 | 制御文字を追加する |
| [FTKR_ExMessageWindow](FTKR_ExMessageWindow.js) | [仮版](FTKR_ExMessageWindow.ja.md) | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExMessageWindow.js) | 2017/03/28 | 制御文字を使って、一度に複数のメッセージウィンドウを表示する |
| [FTKR_ExMessageWindow2](FTKR_ExMessageWindow2.js) | [仮版](FTKR_ExMessageWindow2.ja.md) | [v2.4.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExMessageWindow2.js) | 2017/08/21 | 文章の表示コマンドを使って、一度に複数のメッセージウィンドウを表示する <br> FTKR_ExMessageWindowと組み合わせて使用できません |
| [FTKR_MessageWindowLines](FTKR_MessageWindowLines.js) | なし | [v1.1.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_MessageWindowLines.js) | 2018/02/03 | メッセージウィンドウの行数を変更する<br>文章の表示コマンドを複数組み合わせて４行以上入力可能 |
| [FTKR_PopupSpriteMessage](FTKR_PopupSpriteMessage.js) | なし | [v1.1.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_PopupSpriteMessage.js) | 2018/02/24 | 任意のメッセージを画面上にポップアップ表示する |

[目次に戻る](#目次)

# アイテム_スキル仕様拡張

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ExItemConfig_ItemBasic](FTKR_ExItemConfig_ItemBasic.js) | [仮版](FTKR_ExItemConfig_ItemBasic.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExItemConfig_ItemBasic.js) | 2017/04/29 | アイテムとスキルの基本設定を拡張する |
| [FTKR_ExItemConfig_IB_SkillCost](FTKR_ExItemConfig_IB_SkillCost.js) | [仮版](FTKR_ExItemConfig_IB_SkillCost.ja.md) | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExItemConfig_IB_SkillCost.js) | 2017/04/30 | スキルの消費コストを拡張する <br> ＜以下のプラグインが必要＞<br>[FTKR_ExItemConfig_ItemBasic](FTKR_ExItemConfig_ItemBasic.js) |
| [FTKR_ExItemConfig_Damage](FTKR_ExItemConfig_Damage.js) | [仮版](FTKR_ExItemConfig_Damage.ja.md) | [v1.0.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExItemConfig_Damage.js) | 2017/04/29 | アイテムとスキルのダメージ処理を拡張する |
| [FTKR_ExItemConfig_Effect](FTKR_ExItemConfig_Effect.js) | [仮版](FTKR_ExItemConfig_Effect.ja.md) | [v1.2.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExItemConfig_Effect.js) | 2017/08/27 | アイテムとスキルの使用効果を拡張する |
| [FTKR_ExItemConfig_Activate](FTKR_ExItemConfig_Activate.js) | [仮版](FTKR_ExItemConfig_Activate.ja.md) | [v1.0.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExItemConfig_Activate.js) | 2017/06/23 | アイテムとスキルの発動設定を拡張する |
| [FTKR_ExItemConfig_Required](FTKR_ExItemConfig_Required.js) | [仮版](FTKR_ExItemConfig_Required.ja.md) | [v1.0.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExItemConfig_Required.js) | 2018/02/01 | アイテムとスキルの使用条件を拡張する |

注意）FTKR_ExItemConfig_* と FTKR_SkillExpansion は組み合わせて使用できません。

[目次に戻る](#目次)

# スキル

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_SkillCounter](FTKR_SkillCounter.js) | [あり](FTKR_SkillCounter.ja.md) | [v1.0.5](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SkillCounter.js) | 2017/04/29 | 相手のスキルに対抗して効果を変える |
| [FTKR_SkillSubCommand](FTKR_SkillSubCommand.js) | [仮版](FTKR_SkillSubCommand.ja.md) | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SkillSubCommand.js) | 2017/04/15 | スキル画面にサブコマンドを追加する <br> FTKR_SEP_ShowSkillStatusと組み合わせて使用できません |
| [FTKR_AutoInvokeSkill](FTKR_AutoInvokeSkill.js) | なし | [v1.3.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_AutoInvokeSkill.js) | 2017/11/04 | 特定条件で自動でスキルを発動させる |
| [FTKR_AISkillEvaluate](FTKR_AISkillEvaluate.js) | なし | [v1.2.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_AISkillEvaluate.js) | 2018/01/11 | 自動戦闘時に使用するスキルの評価値を個別に設定する |

## スキル強化システム

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_SkillExpansion](FTKR_SkillExpansion.js) | [仮版](FTKR_SkillExpansion.ja.md) | [v1.3.4](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SkillExpansion.js) | 2017/10/16 | スキルの仕様を拡張する |
| [FTKR_SEP_ShowSkillStatus](FTKR_SEP_ShowSkillStatus.js) | なし | [v1.4.5](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SEP_ShowSkillStatus.js) | 2017/10/19 | スキル画面の表示を拡張する <br> ＜以下のプラグインが必要＞ <br> [FTKR_SkillExpansion](FTKR_SkillExpansion.js) |
| [FTKR_SkillUpgradeSystem_Core](FTKR_SkillUpgradeSystem_Core.js) | [ツクマテ](http://tm.lucky-duet.com/viewtopic.php?f=5&t=3076) | [v1.5.2](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SkillUpgradeSystem_Core.js) | 2017/10/21 | スキル強化システム <br> ＜以下のプラグインが必要＞ <br>[FTKR_SkillExpansion](FTKR_SkillExpansion.js) |
| [FTKR_SkillUpgradeSystem_Window](FTKR_SkillUpgradeSystem_Window.js) | なし | [v1.5.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SkillUpgradeSystem_Window.js) | 2017/10/04 | スキル強化システムの専用画面を実装する <br> ＜以下のプラグインが必要＞ <br>[FTKR_SkillExpansion](FTKR_SkillExpansion.js) <br>[FTKR_SEP_ShowSkillStatus](FTKR_SEP_ShowSkillStatus.js) <br> [FTKR_SkillUpgradeSystem_Core](FTKR_SkillUpgradeSystem_Core.js)|

## スキルツリーシステム

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_SkillTreeSystem](FTKR_SkillTreeSystem.js) | [あり](FTKR_SkillTreeSystem.ja.md) | [v1.14.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SkillTreeSystem.js) | 2018/02/20 | ツリー型のスキル習得システム |
| [FTKR_STS_CustomWindow](FTKR_STS_CustomWindow.js) | [仮版](FTKR_STS_CustomWindow.ja.md) | [v1.2.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_STS_CustomWindow.js) | 2017/06/07 | スキルツリー習得画面のレイアウトを変更する <br> ＜以下のプラグインが必要＞ <br> [FTKR_SkillTreeSystem](FTKR_SkillTreeSystem.js) |

[目次に戻る](#目次)

# アイテム

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ItemNonScope](FTKR_ItemNonScope.js) | [仮版](FTKR_ItemNonScope.ja.md) | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemNonScope.js) | 2017/04/19 | アイテムが範囲なしの場合にパーティーの全メンバーを対象にする |
| [FTKR_ItemCategoryFixed](FTKR_ItemCategoryFixed.js) | [仮版](FTKR_ItemCategoryFixed.ja.md) | [v1.0.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemCategoryFixed.js) | 2017/06/02 | アイテムボックスでカテゴリー選択を無くす |
| [FTKR_ItemSubCommand](FTKR_ItemSubCommand.js) | [仮版](FTKR_ItemSubCommand.ja.md) | [v1.5.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemSubCommand.js) | 2018/02/24 | アイテムボックスにサブコマンドを追加するプラグイン |
| [FTKR_ItemBoxCapacity](FTKR_ItemBoxCapacity.js) | [仮版](FTKR_ItemBoxCapacity.ja.md) | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemBoxCapacity.js) | 2017/06/09 | アイテムボックスに所持容量を追加するプラグイン |
| [FTKR_ItemBoxCategory](FTKR_ItemBoxCategory.js) | [あり](FTKR_ItemBoxCategory.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemBoxCategory.js) | 2017/12/10 | アイテムボックスのカテゴリーを追加変更するプラグイン<br>FTKR_ItemCategoryFixedと組み合わせて使用できません |
| [FTKR_ItemCompositionSystem](FTKR_ItemCompositionSystem.js) | [仮版](FTKR_ItemCompositionSystem.ja.md) | [v1.5.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ItemCompositionSystem.js) | 2017/12/11 | アイテム合成システム |
| [FTKR_ExEquipSlot](FTKR_ExEquipSlot.js) | なし | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExEquipSlot.js) | 2017/12/17 | 同じ装備タイプの装備を２つ以上装備できるようにする |

[目次に戻る](#目次)

# ステート

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_TransformationState](FTKR_TransformationState.js) | なし | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_TransformationState.js) | 2017/10/08 | ステートが掛かっている間SV画像を変更する |
| [FTKR_AutoStateConditions](FTKR_AutoStateConditions.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_AutoStateConditions.js) | 2017/05/02 | ステートに自動付与条件および自動解除条件を設定する |
| [FTKR_ExStateEffects](FTKR_ExStateEffects.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExStateEffects.js) | 2017/08/04 | ステートが掛かっている間に使用したスキルに別のスキルの特徴を追加する |
| [FTKR_ChangeRepeatsState](FTKR_ChangeRepeatsState.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ChangeRepeatsState.js) | 2017/08/23 | ステートが掛かっている間に使用したスキルの連続回数を倍加する |

[目次に戻る](#目次)

# 敵グループ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ExMetaData](FTKR_ExMetaData.js) | [あり](FTKR_ExMetaData.ja.md) | [v1.0.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExMetaData.js) | 2018/02/19 | 敵グループとイベントのメタデータを拡張する |
| [FTKR_SetupTroops](FTKR_SetupTroops.js) | [あり](FTKR_SetupTroops.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_SetupTroops.js) | 2017/05/25 | ゲーム内で敵グループの編成を設定する |

[目次に戻る](#目次)

# バトル

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ExBattleEvent](FTKR_ExBattleEvent.js) | [あり](FTKR_ExBattleEvent.ja.md) | [v1.3.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExBattleEvent.js) | 2018/02/19 | バトルイベントを拡張する |
| [FTKR_DisplayRegenerateMessage](FTKR_DisplayRegenerateMessage.js) | [あり](FTKR_DisplayRegenerateMessage.ja.md) | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_DisplayRegenerateMessage.js) | 2017/05/27 | HP再生量をバトルログに表示する |
| [FTKR_ExBattleCommand](FTKR_ExBattleCommand.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExBattleCommand.js) | 2017/11/25 | バトルコマンドを変更する |
| [FTKR_FVActorAnimation](FTKR_FVActorAnimation.js) | なし | [v1.1.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_FVActorAnimation.js) | 2017/12/25 | フロントビューモードでアクター画像にアニメーションを表示する<br>別途アクター画像表示用のプラグインが必要 |
| [FTKR_BattleAbortConditions](FTKR_BattleAbortConditions.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_BattleAbortConditions.js) | 2018/02/12 | 設定した条件を満たすと、バトルを中断して勝利または敗北する |
| [FTKR_MaxBattleMembers](FTKR_MaxBattleMembers.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_MaxBattleMembers.js) | 2018/02/25 | バトルメンバーの最大人数を変数で管理する |

FTKR_BattleCommandIconはFTKR_ExBattleCommandに統合しました

[目次に戻る](#目次)

# イベント

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_EventSmoothStart](FTKR_EventSmoothStart.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_EventSmoothStart.js) | 2017/06/25 | イベント起動時のプレイヤーの移動停止を無視する |
| [FTKR_EventReSpawnEx](FTKR_EventReSpawnEx.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_EventReSpawnEx.js) | 2017/11/14 | EventReSpawn.jsとTemplateEvent.jsで生成した一時イベントの座標とセルフスイッチを記録する<br> ＜以下のプラグインが必要＞ <br> [EventReSpawn.js(トリアコンタンさんのHPリンク)](https://triacontane.blogspot.jp/2016/08/blog-post.html)  <br>[TemplateEvent.js(トリアコンタンさんのHPリンク)](https://triacontane.blogspot.jp/2016/06/blog-post_25.html) |
| [FTKR_MenuEvent](FTKR_MenuEvent.js) | なし | [v1.0.3](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_MenuEvent.js) | 2018/02/20 | メニュー画面上でコモンイベントを実行する |
| [FTKR_EventMoveByInput](FTKR_EventMoveByInput.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_EventMoveByInput.js) | 2018/01/25 | 指定したイベントを画面の中心にしてキー操作で移動させる |

[目次に戻る](#目次)

# マップ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ExTileSettingForRegion](FTKR_ExTileSettingForRegion.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ExTileSettingForRegion.js) | 2017/08/27 | 指定したリージョンの通行設定を一時的に変更する |

[目次に戻る](#目次)

# セーブ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_DeleteSavefile](FTKR_DeleteSavefile.js) | [仮版](FTKR_DeleteSavefile.ja.md) | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_DeleteSavefile.js) | 2018/02/25 | セーブファイルを削除するコマンドを追加する |

[目次に戻る](#目次)

# ミニゲーム

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_CardGames](FTKR_CardGames.js) | [仮版](FTKR_CardGames.ja.md) | [v1.2.1](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_CardGames.js) | 2017/10/02 | カードゲーム |

[目次に戻る](#目次)

# デバッグ

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_IgnoreScriptError](FTKR_IgnoreScriptError.js) | なし | [v1.0.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_IgnoreScriptError.js) | 2017/05/03 | イベントで実行するスクリプトのエラーを無視する |

[目次に戻る](#目次)

# その他備忘録

* [コードリスト](Code_List.ja.md)

プラグイン対応状況
* スキル強化プラグインの統合(気が向いたら)
* スキルツリープラグインのスキルツリー作成がもう少し簡単にできないか検討(気が向いたら)
* FTKR_OriginalSceneWindowのGDM対応(気が向いたら)

# 試作品置き場

| プラグイン | マニュアル | ダウンロード | 更新日 |  説明 |
|:-----------|:-----------:|:-------------|:-------------|:-------------|
| [FTKR_ActionGauge](FTKR_ActionGauge.js) | なし | [v0.7.0](https://raw.githubusercontent.com/futokoro/RPGMaker/master/FTKR_ActionGauge.js) | 2017/04/21 | アクションゲージ |

# 更新情報

2018/02の更新情報

### 2018/02/25
* [FTKR_MaxBattleMembers](FTKR_MaxBattleMembers.js) v1.0.0(新規)
* [FTKR_DeleteSavefile](FTKR_DeleteSavefile.ja.md) v1.0.0(新規)
* [FTKR_InterlockMouseAndWindow](FTKR_InterlockMouseAndWindow.js) v1.0.0(新規)

### 2018/02/24
* [FTKR_PopupSpriteMessage](FTKR_PopupSpriteMessage.js) v1.1.1
* [FTKR_ItemSubCommand](FTKR_ItemSubCommand.ja.md) v1.5.1
* [FTKR_SceneBackImages](FTKR_SceneBackImages.js) v1.0.0(新規)

### 2018/02/22
* [FTKR_ItemSubCommand](FTKR_ItemSubCommand.ja.md) v1.5.0

### 2018/02/20
* [FTKR_SkillTreeSystem](FTKR_SkillTreeSystem.ja.md) v1.14.0
* [FTKR_MenuEvent](FTKR_MenuEvent.js) v1.0.3

### 2018/02/19
* [FTKR_ExMetaData](FTKR_ExMetaData.ja.md) v1.0.1
* [FTKR_ExBattleEvent](FTKR_ExBattleEvent.ja.md) v1.3.3

### 2018/02/17
* [FTKR_ExTraitSetting](FTKR_ExTraitSetting.js) v1.0.4

### 2018/02/15
* [FTKR_OriginalSceneWindow](FTKR_OriginalSceneWindow.ja.md) v1.5.1

### 2018/02/14
* [FTKR_OriginalSceneWindow](FTKR_OriginalSceneWindow.ja.md) v1.5.0

### 2018/02/13
* [FTKR_SkillTreeSystem](FTKR_SkillTreeSystem.ja.md) v1.13.0

### 2018/02/12
* [FTKR_BattleAbortConditions](FTKR_BattleAbortConditions.js) v1.0.0(新規)

### 2018/02/03
* [FTKR_MessageWindowLines](FTKR_MessageWindowLines.js) v1.1.1

### 2018/02/01
* [FTKR_ItemConfig_Required](FTKR_ExItemConfig_Required.ja.md) v1.0.3

[過去の更新情報](note.md)

#
[目次に戻る](#目次)