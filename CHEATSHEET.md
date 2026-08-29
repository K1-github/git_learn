# Git チートシート（早見表）🧾

## 毎日使う
```bash
git status                 # 今の状態を見る（迷ったらまずこれ）
git add <file>             # 変更をステージング（. で全部）
git commit -m "メッセージ"  # 記録する
git push                   # GitHub に送る
git pull                   # GitHub から取り込む
```

## 確認する
```bash
git diff                   # まだ add していない差分
git diff --staged          # add 済みの差分
git log --oneline          # 履歴を1行ずつ
git log --oneline --graph  # 分岐も図で
```

## ブランチ
```bash
git branch                 # 一覧
git switch -c <name>       # 作って移動
git switch <name>          # 移動
git merge <name>           # 今のブランチに合流
```

## やり直す
```bash
git restore <file>            # add前の編集を取り消す（作業ツリーを戻す）
git restore --staged <file>   # add を取り消す（ステージから外す）
git commit --amend            # 直前のコミットを修正
git revert <commit>           # 特定コミットを打ち消す新コミットを作る
```

## 用語ミニ辞典
| 英語 | 日本語 | ひとこと |
|------|--------|---------|
| repository | リポジトリ | プロジェクトの入れ物 |
| commit | コミット | 記録／セーブ |
| stage / index | ステージ | コミット候補の置き場 |
| branch | ブランチ | 枝分かれした作業 |
| merge | マージ | ブランチを合流 |
| remote / origin | リモート | GitHub 側 |
| push / pull | プッシュ/プル | 送る／取り込む |
| pull request | プルリクエスト | 取り込み提案 |
| conflict | コンフリクト | 変更の衝突 |
