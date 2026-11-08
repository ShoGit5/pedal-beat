# PEDAL BEAT

エレクトーンの**足ペダル**を練習するためのWebアプリです。iPadをエレクトーンにUSBでつなぎ、ブラウザで開いて使います。

- 遊ぶ：https://shogit5.github.io/pedal-beat/
- 方針：[CONSTITUTION.md](CONSTITUTION.md)
- 決めたことの記録：[DECISION_LOG.md](DECISION_LOG.md)

## 使い方
1. エレクトーン（USB TO HOST端子）とiPadをケーブルでつなぐ
2. 上のURLをSafariで開く（「ホーム画面に追加」しておくと便利）
3. 「せってい」→「あわせる」を押して、ペダルのいちばん左のドを踏む
4. 曲を選んで遊ぶ

MIDIが使えない環境でも、画面のペダルをタップするか、Macのキーボード（`a w s e d f t g y h u j k o l p ; '`）で遊べます。

## しくみ
- `index.html` 1ファイルだけで動きます（ビルド不要）
- ELS-02系のMIDIでは、ペダルは3chで送られます
- スコアや自己ベストは、使っている端末のブラウザの中にだけ保存されます（サーバーには送りません）
