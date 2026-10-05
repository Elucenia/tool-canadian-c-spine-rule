<!-- ELUCENIA technical documentation · canadian-c-spine-rule · ja · no clinical/professional/rights approval -->

# Canadian C-Spine Rule

[条件・出典・許諾](https://elucenia.org/ja/tools/canadian-c-spine-rule)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 除外基準：年齢 \< 16歳、Glasgow \< 15、バイタル異常、受傷後48 h超、穿通性外傷、急性麻痺、既知の脊椎疾患・頸椎手術既往、同じ外傷の再診、妊娠

`excl`

### 高リスク：年齢 ≥ 65歳

`idade65`

### 高リスク：危険機転（≥ 0.9 mまたは5段の転落、頭部軸方向負荷、高速衝突、横転・車外放出、動力付きレジャー車両、自転車衝突）

`mecanismo`

### 高リスク：四肢の感覚異常

`parestesia`

### 低リスク：単純な追突（対向車線への押し出し、大型バス・トラックの衝突、横転、高速衝突なし）

`colisao`

### 低リスク：救急室で座位

`sentado`

### 低リスク：受傷後に一度は歩行

`deambulou`

### 低リスク：遅発性頸部痛

`tardia`

### 低リスク：頸椎正中部の圧痛なし

`semdor`

### 自力で頸部を左右それぞれ45°回せますか？

`rot`

任意

- `0` — いいえ
- `1` — はい
- `na` — 未検査

### 鈍的外傷後 ≤ 48 h、年齢 ≥ 16歳、Glasgow 15、バイタル正常、頸部痛または鎖骨上の損傷 + 非歩行 + 危険機転による組入れを確認しましたか？

`contexto`

- `0` — いいえ
- `1` — はい

## 方法の版

Stiell 2001; Canadian C-Spine Rule

## 記載された計算式

手順：除外条件→高リスク因子→低リスク因子の存在→臨床的に評価済みの自動回旋。

## 限界・対象集団

頸部の運動を指示するものではありません。回旋が未評価の場合、結果は不完全となります。基準に該当しないことは損傷がないことを意味しません。

## 参考文献

- [Stiell et al. · Canadian C-Spine Rule · 2001年の論文全文と基準](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
