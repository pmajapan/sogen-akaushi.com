# SEO 対応チェックリスト（草原あか牛HP）

## P0: 公開前 必須対応

### 1. 独自ドメイン取得・接続

- [ ] ドメイン名を決定（例: `sogengyuakagyu.jp`, `sogen-akagyu.com` 等）
- [ ] ドメインを取得（Wix経由 or 外部レジストラ）
- [ ] Wix プレミアムプラン加入（ドメイン接続にはビジネスプラン以上推奨）
- [ ] Wix管理画面 > 設定 > ドメイン から独自ドメインを接続
- [ ] SSL証明書の自動適用を確認（Wixは自動でHTTPS化）

**Wix操作手順**:
1. ダッシュボード > 「設定」 > 「ドメイン」
2. 「ドメインを接続」を選択
3. 外部レジストラの場合: DNS設定でCNAMEレコードを追加

### 2. Wix 広告バナー削除

- [ ] プレミアムプラン加入後、自動的に非表示になることを確認
- [ ] 確認URL: 公開後のサイトでWixバナーが表示されていないことをチェック

### 3. ページタイトル設定

各ページで以下の形式を適用:

| ページ | title タグ |
|--------|----------|
| TOP | `草原あか牛｜阿蘇の大草原で育つ、牛らしい牛` |
| About Us | `私たちについて｜草原あか牛` |
| Restaurant（一覧） | `草原あか牛プレミアムを味わえるレストラン｜草原あか牛` |
| antica locanda MIYAMOTO | `antica locanda MIYAMOTO｜草原あか牛レストラン` |
| 山小屋 Holahoo | `山小屋 Holahoo｜草原あか牛レストラン` |
| 洋食おがた | `洋食おがた｜草原あか牛レストラン` |
| Tradeoff Diner | `Tradeoff Diner｜草原あか牛レストラン` |
| Sustainability | `社会課題への取り組み｜草原あか牛` |
| Story（一覧） | `草原あか牛の牛飼いたち｜草原あか牛` |
| 安藤 大峻 | `安藤 大峻 ― 千葉から阿蘇へ、移住と独立の物語｜草原あか牛` |
| 立脇 良基 | `立脇 良基 ― 牛と米、二足のわらじの放牧生活｜草原あか牛` |
| 飯田 彩華 | `飯田 彩華 ― 牛舎から放牧の道へ｜草原あか牛` |
| Press / Contact | `取材・お問い合わせ｜草原あか牛` |

**Wix操作手順**:
1. エディタ左メニュー > 「ページ・メニュー」
2. 対象ページの「...」 > 「SEOの基本設定」
3. 「タイトルタグ」に上記内容を入力

### 4. meta description 設定

| ページ | meta description（120字以内推奨） |
|--------|-------------------------------|
| TOP | `草原あか牛は阿蘇の大草原で一年中放し飼いで育つあか牛。野草を食み、大地を歩いて育った赤身肉の旨みを、厳選レストランでお届けします。` |
| About Us | `草原を「価値」に変え、未来の食卓へつなぐ。阿蘇の草原を食の源泉として次世代へつなぐ、放牧畜産の専門集団です。` |
| Restaurant | `草原あか牛プレミアムを味わえるレストランをご紹介。肉のマエストロ・新保吉伸氏の手当てを経た最高の赤身肉を一皿に。` |
| Sustainability | `牛も人も草原も。消えゆく阿蘇の草原を放牧で活かし、牛・人・地域に恵みをもたらす循環型の取り組みをご紹介します。` |
| Story | `移住、独立、新規就農。草原あか牛を育む牛飼いたちの挑戦と日常をお伝えします。` |
| Press / Contact | `草原あか牛への取材・講演・お問い合わせはこちら。プレスキット、高解像度写真素材をご用意しています。` |

**Wix操作手順**:
1. 上記タイトルタグと同じ画面（SEOの基本設定）
2. 「ディスクリプション」欄に入力

### 5. OGP（Open Graph Protocol）設定

各ページで以下を設定:

| 設定項目 | 内容 |
|---------|------|
| og:title | 各ページの title タグと同じ |
| og:description | 各ページの meta description と同じ |
| og:image | 各ページのメインビジュアル画像（推奨サイズ: 1200×630px） |
| og:type | `website` |
| og:url | 各ページの正規URL |
| og:site_name | `草原あか牛` |

**Wix操作手順**:
1. SEOの基本設定 > 「ソーシャルシェア」タブ
2. og:title、og:description、og:image を設定
3. Facebook デバッガー（https://developers.facebook.com/tools/debug/）でプレビュー確認
4. Twitter Card Validator でも確認

**OGP画像の準備**:
- [ ] TOP用 OGP画像（1200×630px）: 草原あか牛のメインビジュアル + ロゴ
- [ ] 共通 OGP画像（1200×630px）: 個別設定がないページのフォールバック用
- [ ] 各レストランページ用（任意）: 各店舗の料理写真

---

## P1: 推奨対応

### 6. URLスラッグの最適化

- [ ] 全ページのスラッグを英語に統一（仕様書 01 参照）
- [ ] 日本語スラッグが含まれていないことを確認
- [ ] 不要なデフォルトスラッグ（`/page-1` 等）が残っていないことを確認

### 7. Google Search Console 登録

- [ ] Google Search Console にアクセス（https://search.google.com/search-console/）
- [ ] プロパティを追加（独自ドメイン or URLプレフィックス）
- [ ] Wixでの認証方法:
  1. ダッシュボード > 「マーケティング・SEO」 > 「SEOツール」
  2. 「サイト認証」> Google の認証コードを入力
- [ ] サイトマップ送信: `https://yourdomain.com/sitemap.xml` を登録
- [ ] インデックス状況の確認（公開後）

### 8. 内部リンクの最適化

- [ ] 各ページから関連ページへの相互リンクを確認
- [ ] 孤立ページ（どこからもリンクされていないページ）がないことを確認
- [ ] アンカーテキストにキーワードを含める（「こちら」ではなく「草原あか牛プレミアムについて」等）

### 9. 画像のalt属性設定

全ページの画像に適切な alt テキストを設定:

| 画像の種類 | alt テキスト例 |
|-----------|-------------|
| 草原風景 | `阿蘇の大草原で放牧される草原あか牛` |
| 牛のアップ | `野草を食む草原あか牛` |
| 肉の写真 | `草原あか牛プレミアムの赤身肉` |
| 新保氏 | `肉のマエストロ 新保吉伸氏` |
| 各シェフ | `antica locanda MIYAMOTO オーナーシェフ 宮本健真氏` |
| 料理写真 | `草原あか牛プレミアムを使用した antica locanda MIYAMOTO の一皿` |

**Wix操作手順**:
1. エディタで画像を選択
2. 「設定」アイコンをクリック
3. 「画像についての説明を追加しましょう」欄に alt テキストを入力

### 10. 構造化データ（Schema.org）

WixではカスタムHTMLの追加が可能。以下のスキーマを検討:

**Organization（TOPページ）**:
```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "草原あか牛",
  "url": "https://yourdomain.com",
  "logo": "https://yourdomain.com/logo.png",
  "description": "阿蘇の大草原で一年中放し飼いで育つあか牛のブランド",
  "address": {
    "@type": "PostalAddress",
    "addressRegion": "熊本県",
    "addressLocality": "阿蘇郡"
  }
}
```

**Restaurant（各レストランページ）**:
```json
{
  "@context": "https://schema.org",
  "@type": "Restaurant",
  "name": "antica locanda MIYAMOTO",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "熊本市",
    "addressRegion": "熊本県"
  },
  "servesCuisine": "イタリアン",
  "chef": {
    "@type": "Person",
    "name": "宮本 健真"
  }
}
```

**Wix操作手順**:
1. ダッシュボード > 「マーケティング・SEO」 > 「SEOツール」
2. 「構造化データマークアップ」を選択
3. 対象ページを選び、上記JSONを貼り付け

---

## チェック完了確認

公開前に以下のツールで最終確認:

- [ ] Google Rich Results Test（https://search.google.com/test/rich-results）で構造化データ確認
- [ ] PageSpeed Insights（https://pagespeed.web.dev/）でパフォーマンス確認
- [ ] Facebook Sharing Debugger で OGP 確認
- [ ] モバイルフレンドリーテスト（Google Search Console内）
- [ ] 全ページのリンク切れ確認
