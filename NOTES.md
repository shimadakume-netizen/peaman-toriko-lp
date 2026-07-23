# LP制作メモ（NOTES.md）

## プロジェクト
- フォルダ: `peaman-toriko-lp`（半角英数）
- 目的: note記事「読まれない文章の正体 ― 7つのライティング逆説」（商品名: 虜ライティング）への誘導
- 記事URL（CTAリンク先）: https://note.com/pman1212/n/nbdcb92e91212
- 元原稿: `C:\Users\seiya\OneDrive\ドキュメント\虜ライティング.pdf`（45ページ・全文はscratchpadのtoriko.txtに抽出済み）

## 決まったこと
- **ターゲット**: ライティング教材を真面目に学んできたのに、スキもコメントも来ない人
- **ヒーローコピー**: 「いい文章を書こう」と思った瞬間、もう負けています。（記事冒頭そのまま／「もう負けています。」を朱で強調）
- **デザイン**: A=文学的な"原稿とインク"の世界観。生成り(#f6f1e5)×墨(#2b2620)×朱(#c73e3a)。Shippori Mincho。原稿用紙の方眼をうっすら・インク染み・朱印「虜」がスタンプアニメで押される・縦書き「読まれない文章の正体」(モバイル非表示)
- **構成**: ヘッダー → ヒーロー → 共感(真面目に学んだのに…破線区切りリスト) → 7つの逆説(世間のコツに取り消し線→朱の逆説「弱さを書け」等7項目→「全部、逆です。」) → ビフォーアフター(いい話モードA vs 弱さモードB・記事の実例) → 結論「文章は正しさではなく揺らぎで届く」 → CTA「不完全なまま、出す。」 → フッター
- **アニメ**: 墨が滲むreveal(blur→クリア)・朱印スタンプ・ボタン控えめシャイン・朱の読み進みバー。prefers-reduced-motion対応
- **キャラ**: peaman.png（ヘッダー/フッターのみ。文学世界観なので控えめ）
- **フッター**: note https://note.com/pman1212 / Threads https://www.threads.com/@pmen.1212 / 記事リンク

## 注意（過去の学び）
- Vercel CLIは表示名「たけし」(日本語)バグで使用不可 → GitHub push→Vercelダッシュボード連携（初回のみユーザーがImport 3クリック）
- OneDrive配下のfile://プレビューは静的スナップショット → 確認は `python -m http.server` 経由

## つづきのメモ
- [x] LP本体作成完了
- [x] セルフチェック済み（自己採点8.5点）: 画像/リンク/フォント/7逆説/朱印OK・overflow-x:clip対策済み。※プレビュー非表示のため見た目の最終確認は未（幅0で測定不可）→ユーザーの目視確認待ち
- [x] GitHub push済み（repo: shimadakume-netizen/peaman-toriko-lp）
- [x] Vercel公開完了: https://peaman-toriko-lp.vercel.app
      ※今回は**Claude がユーザーのChromeを操作して Import→Deploy を代行**できた（claude-in-chrome MCP接続済み・Vercelログイン済みだったため）。今後のデプロイもこの方法でAI代行可能。以後の更新はgit pushだけで自動反映
