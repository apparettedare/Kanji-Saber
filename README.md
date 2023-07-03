# 漢字セイバーのセットアップ

漢字セイバーのセットアップ方法を記述します．

## Unityのインストール
- [ここ](https://unity.com/ja/download)からUnityをインストール．
- OSとUnityのバージョンは以下の通りです．

| 番号 | アイテム       | 説明    |
|:--:| ---------- |----------------|
| 1  | OS         | Windows10    |
| 2  | Unity      | [Unity 2020.3.26f1](https://unity.com/releases/editor/whats-new/2020.3.26) |

## 漢字セイバープロジェクトの作成方法  

1. Unity Hubを開いて，新しいプロジェクトを作成してください．
1. プロジェクト名と保存先を選んで作成．
1. 作成出来たらAssets -> Import Package -> Custom Packageを選択してダウンロードしたファイルを選択.  
1. Importできたら　File　-> Build Settings を選択してAdd Open Scenesで以下のように順番通りに追加
    1. Title
    1. Login
    1. Quiz
    1. Result
    1. Score
1. プロジェクトファイルの中にKanjiConfigをペースト．


### VOICE VOXのインストール

- 動物やナレーションの声を作成してくれる[VOICEVOX](https://voicevox.hiroshiba.jp/)というアプリをインストールします.  
- 画像のように選択してインストールしてください．  
![スクリーンショット 2023-06-29 185217](https://github.com/apparettedare/Kanji-Saber/assets/87752284/fa47630b-595d-4c7a-9b7d-d00ac59f02f8)
- ファイルを開き，run.exeを起動する．
- [このリンク](http://localhost:50021/docs)がブラウザで表示できることを確認してください．
- 漢字セイバーを起動するときは必ずrun.exeも起動しておいてください.
最後に何もエラーが起こっていないことを確認してTitleシーンを選択し再生ボタンを押してください．  
## 問題作成方法
- KanjiConfigフォルダーの中にKanjiConfig.json, QuestionInfo.json, KanjiImageフォルダーの三つの要素があります．
- KanjiConfig.jsonのmaxNumberOfQuestionには問題数を入力してください.
- QuestionInfo01.json, QestionInfo02.jsonのようにQustionInfo + 二桁の整数 + .jsonという名前にしてQuestionInfo.jsonファイルを作成してください．
    - quiz_text: 問題にしたい漢字
    - part_text: 問題にしたい漢字の部首
    - answer_text: 問題の答えとなる漢字
    - dummy1_text: 問題の答えにならない漢字
    - dummy2_text: 問題の答えにならない漢字
    - ○○○○_kanji:  それぞれひらがなで入力していたものを漢字で入力（発話指定のため）
- KanjiImageフォルダーの中にImage01, Image02のようにフォルダーを作成し，その中にQuestionInfo.jsonファイルで定義した漢字と対応するイメージを入れてください．
- Imageの中に入るファイルの名前はそれぞれの漢字の名前（ひらがな）と対応するようにしてください．
    - 動画ファイルの拡張子はm4v
    - 画像ファイルの拡張子はjpg
-[参考](http://www3.u-toyama.ac.jp/raicho/textbook/) 
