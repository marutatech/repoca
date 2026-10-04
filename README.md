# Repoca 公式Webサイト

GitHub Pagesで公開できる、Repoca（レポカ）の静的ランディングページです。フレームワークやビルド処理は不要です。

## ローカル確認方法

最も簡単な確認方法は `index.html` をブラウザで開く方法です。ローカルサーバーで確認する場合は、このディレクトリで次のいずれかを実行します。

```powershell
python -m http.server 8000
```

その後、ブラウザで `http://localhost:8000/` を開きます。

## 画像の差し替え

画像は `assets/images/` にまとめています。現在のファイル名を維持したまま同じ縦横比の画像へ差し替えると、HTMLを変更せずに更新できます。

- `repoca-hero.png`: 正式メインビジュアル（1672×941px）
- `repoca-app-icon.png`: ヘッダー／フッター用のRepoca正式アイコン（1254×1254px）
- `repoca-app-flow.png`: 撮影から報告書完成までの4画面画像（1774×887px）
- `Download_on_the_App_Store_Badge_JP_RGB_blk.svg`: Apple公式の日本語版App Store黒バッジ
- `GetItOnGooglePlay_Badge_Print_color_Japanese.svg`: Google公式の日本語版Google Play SVGバッジ（公式配布アーカイブ内のWeb用SVG）
- `building-maintenance.png`: ビルメンテナンス画像
- `equipment-inspection.png`: 設備点検画像
- `landscape-management.png`: 植栽管理画像
- `construction-repair.png`: 工事・修繕画像
- `repoca-ogp.png`: 正式OGP画像（1200×630px）

「Repoca」のブランド名はHTMLテキスト、アイコンは `repoca-app-icon.png` を使用しています。

## 設定済みURL

- App Store: `https://apps.apple.com/jp/app/repoca-%E3%83%AC%E3%83%9D%E3%82%AB-%E5%86%99%E7%9C%9F%E4%BB%98%E3%81%8D%E4%BD%9C%E6%A5%AD%E5%A0%B1%E5%91%8A%E6%9B%B8/id6789023940`
- Google Play: `https://play.google.com/store/apps/details?id=jp.co.daisei.repoca`
- Instagram: `https://www.instagram.com/repoca.app/`
- プライバシーポリシー: `https://marutatech.github.io/repoca-support/privacy.html`
- 公式Webサイト: `https://marutatech.github.io/repoca/`
- OGP画像: `https://marutatech.github.io/repoca/assets/images/repoca-ogp.png`

canonical、`og:url`、`og:image`、Twitter Cardは正式公開URLに設定済みです。

ストアバッジはApple DeveloperのApp Storeマーケティングツール、およびGoogle Partner Marketing Hubの公式配布素材を使用しています。

## 公開対象

GitHub Pagesのサイト本体として公開する対象は次のとおりです。

- `index.html`
- `styles.css`
- `assets/`（未使用の旧OGPプレースホルダーを除く）

リポジトリ管理用として、次のファイルもGitHubへ追加できます（ページ本体からは参照しません）。

- `README.md`
- `.gitignore`

`work/`、`outputs/`、テスト用スクリーンショット、確認用スクリプト、ZIP、一時ファイルは公開対象外です。既存の作業ファイルは削除せず、`.gitignore`で新規リポジトリの追跡対象から除外します。

Webサイト対応版の`privacy.html`はまだ公開せず、公式サイトからは引き続き`https://marutatech.github.io/repoca-support/privacy.html`を参照します。

## GitHub Pages公開方法

1. 公開対象ファイルだけをGitHubリポジトリへ追加します。
2. GitHubのリポジトリ画面で **Settings → Pages** を開きます。
3. **Build and deployment** のSourceを **Deploy from a branch** にします。
4. 公開対象ブランチ（通常は `main`）とフォルダ `/ (root)` を選択して保存します。
5. 表示された公開URLでページと各リンクを確認します。

このリポジトリからの公開操作は自動では行いません。

## 公開前チェック

- 実機（iPhone / Android）での最終表示確認
