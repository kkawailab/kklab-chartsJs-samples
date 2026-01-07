# Chart.js サンプル集

Chart.js を使った30個のサンプルファイル集です。初心者から上級者まで段階的に学習できるように構成されています。

## 学習ガイドブック

本サンプル集には、詳細な解説付きの学習ガイドブック（PDF）が付属しています。

**[Chart.js 学習ガイドブック（PDF）](guide/chartjs-guide.pdf)**

ガイドブックの内容：
- **第I部（01-10）**: 初心者レベル - 基本的なチャートタイプの作成
- **第II部（11-20）**: 中級レベル - カスタマイズとスタイリング
- **第III部（21-30）**: 上級レベル - インタラクティブ機能とダッシュボード
- **第IV部**: LLM活用学習ガイド - ChatGPT/Claude等を使った効率的な学習プロンプト集

## 使い方

各サンプルは単一のHTMLファイルで完結しています。ブラウザで直接開くだけで動作します。

```bash
# 例: サンプル01を開く
open samples/01-basic-line-chart.html
```

## ディレクトリ構成

```
kklab-chartsJs-samples/
├── guide/                  # 学習ガイドブック
│   └── chartjs-guide.pdf   # PDF（165ページ）
├── samples/                # サンプルHTML（30ファイル）
├── index.html              # GitHub Pages
└── README.md
```

## Chart.js について

- **公式サイト**: https://www.chartjs.org/
- **ドキュメント**: https://www.chartjs.org/docs/latest/
- **使用バージョン**: 4.4.1（CDN経由）

---

## 目次

### 初心者レベル（01-10）

基本的なチャートの作成方法を学びます。

| No. | ファイル名 | 内容 | 学習ポイント |
|-----|-----------|------|-------------|
| 01 | [01-basic-line-chart.html](samples/01-basic-line-chart.html) | 基本的な折れ線グラフ | Chart.jsの基本的な使い方、type: 'line' |
| 02 | [02-basic-bar-chart.html](samples/02-basic-bar-chart.html) | 基本的な棒グラフ | type: 'bar'、borderRadius |
| 03 | [03-horizontal-bar-chart.html](samples/03-horizontal-bar-chart.html) | 横棒グラフ | indexAxis: 'y' で横向きに |
| 04 | [04-basic-pie-chart.html](samples/04-basic-pie-chart.html) | 基本的な円グラフ | type: 'pie'、割合の自動計算 |
| 05 | [05-doughnut-chart.html](samples/05-doughnut-chart.html) | ドーナツチャート | type: 'doughnut'、cutout設定 |
| 06 | [06-radar-chart.html](samples/06-radar-chart.html) | レーダーチャート | type: 'radar'、複数指標の比較 |
| 07 | [07-multi-line-chart.html](samples/07-multi-line-chart.html) | 複数データセットの折れ線グラフ | 複数のdatasets、凡例 |
| 08 | [08-grouped-bar-chart.html](samples/08-grouped-bar-chart.html) | グループ化された棒グラフ | 複数データセットの棒グラフ |
| 09 | [09-stacked-bar-chart.html](samples/09-stacked-bar-chart.html) | 積み重ね棒グラフ | stacked: true |
| 10 | [10-area-chart.html](samples/10-area-chart.html) | エリアチャート | fill: true で塗りつぶし |

---

### 中級レベル（11-20）

様々なチャートタイプとカスタマイズ方法を学びます。

| No. | ファイル名 | 内容 | 学習ポイント |
|-----|-----------|------|-------------|
| 11 | [11-scatter-chart.html](samples/11-scatter-chart.html) | 散布図 | type: 'scatter'、{x, y}形式のデータ |
| 12 | [12-bubble-chart.html](samples/12-bubble-chart.html) | バブルチャート | type: 'bubble'、{x, y, r}形式 |
| 13 | [13-polar-area-chart.html](samples/13-polar-area-chart.html) | 極座標エリアチャート | type: 'polarArea' |
| 14 | [14-mixed-chart.html](samples/14-mixed-chart.html) | 複合チャート（棒と線） | データセットごとに異なるtype |
| 15 | [15-stepped-line-chart.html](samples/15-stepped-line-chart.html) | ステップ線グラフ | stepped: 'before'/'after'/'middle' |
| 16 | [16-gradient-background.html](samples/16-gradient-background.html) | グラデーション背景 | Canvas APIのcreateLinearGradient |
| 17 | [17-custom-tooltip.html](samples/17-custom-tooltip.html) | ツールチップのカスタマイズ | tooltip.callbacks |
| 18 | [18-custom-legend.html](samples/18-custom-legend.html) | 凡例のカスタマイズ | カスタムHTML凡例、クリックイベント |
| 19 | [19-custom-axes.html](samples/19-custom-axes.html) | 軸のカスタマイズ | ticks.callback、グリッド設定 |
| 20 | [20-data-labels.html](samples/20-data-labels.html) | データラベルの表示 | chartjs-plugin-datalabels |

---

### 上級レベル（21-30）

高度な機能とインタラクティブな実装を学びます。

| No. | ファイル名 | 内容 | 学習ポイント |
|-----|-----------|------|-------------|
| 21 | [21-realtime-update.html](samples/21-realtime-update.html) | リアルタイムデータ更新 | data.push()、chart.update() |
| 22 | [22-drilldown.html](samples/22-drilldown.html) | ドリルダウン機能 | クリックで詳細データを表示 |
| 23 | [23-custom-plugin.html](samples/23-custom-plugin.html) | カスタムプラグイン | beforeDraw/afterDrawフック |
| 24 | [24-custom-animation.html](samples/24-custom-animation.html) | アニメーションのカスタマイズ | easing、duration、delay |
| 25 | [25-dual-y-axis.html](samples/25-dual-y-axis.html) | 複数Y軸 | 複数のscales、yAxisID |
| 26 | [26-html-tooltip.html](samples/26-html-tooltip.html) | HTML カスタムツールチップ | tooltip.external |
| 27 | [27-click-events.html](samples/27-click-events.html) | クリックイベント処理 | onClick、getElementsAtEventForMode |
| 28 | [28-export-image.html](samples/28-export-image.html) | チャートを画像としてエクスポート | canvas.toDataURL() |
| 29 | [29-responsive-design.html](samples/29-responsive-design.html) | レスポンシブデザイン | responsive、maintainAspectRatio |
| 30 | [30-dashboard.html](samples/30-dashboard.html) | ダッシュボード（複数チャート） | 複数チャートの統合、ダークテーマ |

---

## チャートタイプ一覧

| チャートタイプ | 説明 | サンプル |
|--------------|------|---------|
| `line` | 折れ線グラフ | 01, 07, 10, 15, 16 |
| `bar` | 棒グラフ | 02, 03, 08, 09 |
| `pie` | 円グラフ | 04 |
| `doughnut` | ドーナツチャート | 05, 23 |
| `radar` | レーダーチャート | 06 |
| `scatter` | 散布図 | 11 |
| `bubble` | バブルチャート | 12 |
| `polarArea` | 極座標エリアチャート | 13 |

---

## 主な学習トピック

### 基本設定
- チャートの作成と初期化
- データ構造（labels、datasets）
- オプション設定

### スタイリング
- 色の設定（backgroundColor、borderColor）
- グラデーション
- フォント設定

### インタラクション
- ツールチップ
- 凡例
- クリックイベント
- ホバーエフェクト

### 軸とスケール
- 軸のカスタマイズ
- 複数軸
- グリッド設定

### アニメーション
- イージング関数
- 遅延アニメーション
- 更新アニメーション

### 高度な機能
- プラグイン開発
- リアルタイム更新
- データのエクスポート
- レスポンシブ対応

---

## 必要な外部ライブラリ

すべてのサンプルはCDN経由でライブラリを読み込んでいます（バージョン固定）。

```html
<!-- Chart.js本体（v4.4.1） -->
<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.1/dist/chart.umd.min.js"></script>

<!-- データラベルプラグイン（サンプル20で使用） -->
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-datalabels@2.2.0"></script>
```

---

## 著者

河合勝彦
名古屋市立大学大学院経済学研究科
kkawai@econ.nagoya-cu.ac.jp

## ライセンス

このサンプル集は学習目的で作成されています。
Chart.js は MIT ライセンスで公開されています。
