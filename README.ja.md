# XXD Panel 120｜建築コンセプト手描き帖

写真の空間的な記憶を、余白豊かな建築スケッチへ。

[简体中文](README.md) · [English](README.en.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [العربية](README.ar.md)

## 作例

8 枚の作例は異なるフォルダの原写真を参照し、Panel 120 が各画像を独立した一回の生成で制作します。写真に基づく英語の文章を使い、公開前に AI メタデータを除去します。横長は左に写真・右にデザイン、縦長は上に写真・下にデザインを各 50% 配置します。

**16:9 · left-right · 50:50**

| sample-05 | sample-06 |
|---|---|
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |

**3:4 · top-bottom · 50:50**

| sample-09 | sample-10 |
|---|---|
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 適した用途と解決する課題

写真全体をなぞらず、設計を検討する感覚のあるコンセプト図にしたいときに。Panel 120 は写真の同一性と空間的な記憶を保ち、核となる形態、輪郭、関係を自由な透視線画に精選します。少量の色面、幾何学的な参照線、大量の余白が作品を構成します。

### 適している場面

- 建築、空間、旅行、物の写真を編集的なコンセプト手描きにしたい。
- 弱い構図、乱れた背景、小さな被写体を削減、再配置、尺度変更で立て直したい。
- 全面着彩や写実的な完成予想図にせず識別性と空間関係を残したい。
- 対照構図、デザインのみ、壁紙、フォルダ一括出力で同じ様式を使いたい。

### 解決すること

- 背景と副次的な物を省き、主要な形態と視覚的な記憶を残します。
- 抑制された、わずかに反復する透視線と構築線で設計探索を表します。
- 装飾で画面を埋めず、余白を構図の一部にします。
- 対照図は等分した二領域のみとし、各原写真から独立生成して二重の様式化を避けます。

## 原文プロンプト · 5 言語

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中国語版はユーザーの原文を逐語保存し、実行時の唯一の創作・美的基準です。他の版は完全で忠実な閲覧用翻訳です。

建築コンセプト透視スケッチ · 手描き線画 · 幾何学的参照線 · 少量の色と影 · 写真由来の 2–4 色 · 大量の余白 · 最小限の編集的注記

## 写真から作品への流れ

主題と空間関係を理解 → 核となる形態を精選 → 複雑な背景を削除 → 尺度と切り取りを再構成 → 透視線・幾何学的参照線・少量の色面で再構築 → 余白と短い注記で仕上げ

## 仕上がりの特徴

- 写真を上または左に残し、軽い色調整のみで同一性と姿勢を維持します。
- デザインは建築コンセプト手描きであり、全景の写し、写実的完成図、3D ではありません。
- 小さく精選した被写体は偏心、端寄せ、部分裁断ができ、余白が構図に参加します。
- 原写真の 2–4 色を清潔で抑制された配色にし、要所だけ薄く置きます。
- 幾何学的な影で量感と奥行きを示し、少数の補助線で検討の感覚を残します。
- 少量の文字を余白に静かに置き、固定書体テンプレートは使いません。作例は英語です。

選択した交付モードは配置だけを変え、原文の美的要件は維持します。`left-right` は上の写真を左、下のデザインを右に映します。指定比率は原文の既定 `3:4` に優先します。

## 4つの出力モード

- `top-bottom`：全幅の上下2領域のみ。実写を上、デザインを下に置き、各50%。
- `left-right`：全高の左右2領域のみ。実写を左、デザインを右に置き、各50%。上下構成へ回転しません。
- `design-only`：全画面を Panel 120 のデザイン翻訳にし、写真は見えない参照にします。
- `wallpaper-pack`：スマートフォン、iPad、デスクトップ、時計を端末ごとに生成。`linked` または `independent` を選べます。

モードと比率は複数指定できます。`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5`、正確なピクセルに対応します。文字はプロンプト生成、指定文の逐字使用、なしから選べます。フォルダ入力では各画像を分離して処理し、PNGを一つの新しいタスクフォルダへ置きます。

## はじめに

```bash
git clone https://github.com/nevertoday/xxd-panel-120.git
npx skills add https://github.com/nevertoday/xxd-panel-120 --skill xxd-panel-120
```

インストール後に Agent セッションを再起動し、`$xxd-panel-120` を呼び出します。ユーザー単位の Codex には `--global --agent codex --yes` を追加できます。

```text
/xxd-panel-120 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale ja-JP
/xxd-panel-120 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-120 photo.jpg --mode design-only --size 9:16 --text none
```

完全な実行契約は [SKILL.md](SKILL.md)、実行アダプターは[英語](references/xxd-panel-120-prompt.en.md)／[中国語](references/xxd-panel-120-prompt.zh-CN.md)を参照してください。

<!-- xxd-readme-ads:start -->
## XXD について

XXD は Xiaoxiaodong のブランド名略称です。作成・管理： [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## サポートとメンバーシップ

> **広告表示：** このセクションのQRコードおよび有料会員・サービスのリンクはXXDのプロモーション情報です。スキャンや購入は任意であり、オープンソースの利用には影響しません。


<!-- xxd-panel-command-system:start -->

すべての将軍 Skills は年額 CNY 699 の共通会員特典に含まれ、別途購入は不要です。

| 階級 | Skill | 担当 |
|---|---|---|
| **将軍級** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 利用可能な番号付き Skills の検出、画像・テーマ・用途からの推薦、番号指定の派遣、同一素材の複数スタイル試作、フォルダー画像の一括割り当てと個別派遣。 |
| **兵士級** | `xxd-panel-NNN` | 各番号が固有の原文プロンプトと美学だけを実行し、将軍から渡された一つの仕事を完成させます。 |

<!-- xxd-panel-command-system:end -->

### 知識星球＋会員プロンプトライブラリ＋全将軍 Skills 会員 · 年額 CNY 699

[知識星球](https://wx.zsxq.com/group/15554814142882)、[XXD 会員プロンプトライブラリ](https://vip.xiaoxiaodong.ai/)、全将軍 Skills 会員は同じ会員権です。**一度の年額決済で3つの特典をすべて利用でき、二重の購入は不要です。**

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) · [Member Prompt Library](https://vip.xiaoxiaodong.ai/)

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD WeChat" width="280"></a></p>

---

<div align="center">

## ☕ オープンソースを支援

このプロジェクトが役に立ったら、Buy Me a Coffee から任意で応援していただけます。

<p align="center"><a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Buy Me a Coffee" width="180"></a></p>

</div>
<!-- xxd-readme-ads:end -->

## ライセンス

本プロジェクト（Skill、プロンプト、スクリプト、文書、付属サンプル画像を含む）は **PolyForm Noncommercial License 1.0.0** の下で提供されます。完全な法的条文は [LICENSE](LICENSE)、公式ページは <https://polyformproject.org/licenses/noncommercial/1.0.0> を参照してください。

分かりやすく言うと：

- 個人は学習、研究、実験、テスト、趣味のプロジェクト、私的娯楽に使用できます。慈善団体、教育機関、公的研究・安全・保健機関、環境保護団体、政府機関も使用できます。
- **非商業目的**であれば、使用、複製、変更、派生物の作成、共有が可能です。共有時には本ライセンス（または上記リンク）と、作者が示したすべての `Required Notice:` 文を添付する必要があります。
- 商用製品・サービス、有料納品、アクセス権やライセンスの販売、商業利用につながることが予想される用途には使用できません。商用利用には著作権者から別途書面による許可を得てください。
- 本契約が付与するのは明記された著作権ライセンスと限定的な特許ライセンスだけです。商標、ブランド名、その他明記されていない権利は付与されず、ライセンスを第三者へ再許諾することもできません。
- 書面で違反通知を受けた場合、32 日以内に遵守状態へ戻り、実際の是正措置を取らなければライセンスは直ちに終了します。特許侵害を書面で主張した場合も特許ライセンスが終了します。
- 内容は法律が認める範囲で「現状のまま」提供され、保証はありません。利用に伴うリスクと損失は利用者が負います。
