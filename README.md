# Downloads — takumi ichimura

Windows向けのゲーム実行版と、Rust製GameEngineのエディター・公式サンプルを配布しています。ソースコードはこのリポジトリに含めていません。

## ダウンロード

ZIPをダウンロードして**すべて展開**し、同梱の起動ファイルを実行してください。ZIPを開いたまま実行せず、画像・音・DLLなどを同じフォルダーに残してください。

| 作品 | 対応環境 | ZIP | 起動ファイル |
| --- | --- | --- | --- |
| GameEngine | Windows 10 / 11（64bit） | [ダウンロード — 49.0 MB](https://github.com/KdGithubIt/portfolio-downloads/releases/download/v2026.10.19/GameEngine-Windows-x64-v2026.10.19.zip) | `Play-TinyGoal.cmd` |
| コマンドRPG | Windows 10 / 11（64bit） | [ダウンロード — 110.8 MB](https://github.com/KdGithubIt/portfolio-downloads/releases/download/v2026.10.19/Command-RPG-Windows-x64-v2026.10.19.zip) | `Play.cmd` |
| Cockpit on Knife Edge | Windows 10 / 11（32bit / 64bit） | [ダウンロード — 51.5 MB](https://github.com/KdGithubIt/portfolio-downloads/releases/download/v2026.10.19/Cockpit-on-Knife-Edge-Windows-x86-v2026.10.19.zip) | `Play.cmd` |

[すべての配布ファイル・リリース情報](https://github.com/KdGithubIt/portfolio-downloads/releases/tag/v2026.10.19)

GitHubが表示する「Source code」のZIPは配布用のゲームではありません。上のリンクか、Releases内の作品名付きZIPを使用してください。

## 遊び方

- **Cockpit on Knife Edge**: Enterで開始。方向キーで移動、Zで通常弾、Xでチャージ弾、Cでスタン弾。
- **コマンドRPG**: 左右で移動、上でジャンプ、Spaceで回転、Zで攻撃。戦闘は上下とEnterで選択・決定。
- **GameEngine / Tiny Goal**: `Play-TinyGoal.cmd`を実行。W/A/S/Dで青いキューブを動かし、金色のキューブに触れるとクリア。`Open-Editor.cmd`で同梱サンプルを指定してエディターを開けます。

GameEngineのサンプルを遊ぶためにRustやビルド環境は不要です。新しいRustコードをビルドする場合は別途RustツールチェーンとエンジンSDKが必要です。詳しい操作は各ZIPの`README.txt`を参照してください。

## 配布内容と確認範囲

実行ファイル、必要なゲームデータ、起動用CMD、操作説明、ライセンス表示を同梱しています。エンジンは開発中です。

同梱ファイルの検証、ZIPのCRC検査、Windows環境での起動確認を実施しています。エンジンの公式サンプルではコンパイル済みゲームモジュールを読み込み、180フレームの実行処理も確認しました。全ステージの通しプレイや、別PCでの確認は未実施です。

CoopQuestは配布準備中です。

## 整合性の確認

[SHA256SUMS.txt](SHA256SUMS.txt)に各ZIPのSHA-256を掲載しています。PowerShellでは次のコマンドで確認できます。

```powershell
Get-FileHash -Algorithm SHA256 .\ダウンロードしたファイル.zip
```

作品一覧の機械可読データは[downloads.json](downloads.json)です。

ゲームの画像・音・フォントや第三者ライブラリの権利は、それぞれの権利者に帰属します。各配布物のライセンス表示を参照してください。エンジンと公式サンプルは同梱のMITまたはApache-2.0ライセンスに従います。

[GitHubプロフィール](https://github.com/KdGithubIt)
