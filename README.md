# MyBeatSaberAnalytics

### [For English user(MyBSAnalytics_Lite: Ranked Score only & English ver.)](https://github.com/hatopopvr/MyBSAnalytics_Lite)

## 概要
BeatSaberの[ScoreSaber](https://scoresaber.com/)の情報を取得し、Rank譜面Clearの進捗状況や、Play傾向を散布図で分析するツールです。

本ツールは [Satoさん](https://twitter.com/zitasato) の [MyBeatSaberScore](https://github.com/tkns3/MyBeatSaberScore/) に影響を受け、クリア進捗やスコア傾向をグラフ等で可視化するために作成しました。  本ツールには未クリア譜面の詳細検索や未クリア譜面のプレイリスト作成機能などは含まれません。

## 使用方法
以下リンクより該当する notebook をGoogle Colobで起動してください。   

- [通常版](https://colab.research.google.com/github/hatopopvr/MyBeatSaberAnalytics/blob/main/MyBeatSaberAnalytics.ipynb): ScoreSaberのアカウントが要ります。曲データは以下の使用データを参照ください。
- [Beta v0.0.6](https://colab.research.google.com/github/hatopopvr/MyBeatSaberAnalytics/blob/main/MyBeatSaberAnalytics_20230825_Beta_0_0_6.ipynb): ベータ版。上記に加えてBeatLeaderのデータを追加で取得するため、BeatLeaderアカウントが要ります。
- [MyBSAnalytics_Lite](https://colab.research.google.com/github/hatopopvr/MyBSAnalytics_Lite/blob/main/MyBSAnalytics_Lite_En.ipynb): Lite版。ScoreSaberのアカウントが要ります。曲データはランク譜面のみを取り扱います。

入力情報のフォームに必要事項を入力し、ランタイムでセルを実行してください。  
セルを実行していただくと、Google Driveにマウントし、曲情報やPlay情報などをGoogle Driveの指定フォルダに保存します。  
プレイ情報と曲情報の取得・解析には時間がかかります。  

Rank譜面のClearの進捗状況や、SS/S/AなどのScoreのランクの状況を可視化できます。

<img src="https://pbs.twimg.com/media/FPBJ8_xacAU9rNA?format=jpg" />

条件を選択し散布図で分析できます。

<img src="https://pbs.twimg.com/media/FO8HJb1agAcVvn5?format=jpg" />

## 使用データ
本ツールは以下のデータを利用しています。
- ScoreSaberのPublic API - [doc](https://docs.scoresaber.com/)  
　Player情報 - https://scoresaber.com/api/player/{player_id}/full  
　Score情報 - https://scoresaber.com/api/player/{player_id}/scores?sort=recent&page={page}  
- BeatLeader API (Betaのみ) - [doc](https://api.beatleader.xyz/swagger/index.html)  
　Score情報 - https://api.beatleader.xyz/player/{player_id}/scores
- 画像データ  
　Player画像 - https://cdn.scoresaber.com/avatars/{player_id}.jpg  
　Cover画像 - https://cdn.scoresaber.com/covers/{hash}.png  
- 曲情報  
  暫定的ですがandruzzzhkaさんがgithubで公開している[
BeatSaberScrappedData](https://github.com/andruzzzhka/BeatSaberScrappedData) を利用しています。

## 使用ライブラリ

本ツールは多数のOSSのLibraryに依存しています。
使用項目については Libraryの取得 を参照願います。

## 問い合わせ先

twitter:[@hatopop_vr](https://twitter.com/hatopop_vr)
