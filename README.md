# 気象条件とコロナウイルスの感染者数の関係性の調査
### 目的
コロナ感染者数と気象の関係を分析し、感染者数の増減に影響を与える気象要素の推定

### 条件
- 調査は東京の2020年と2021年に限定
- 気象データは気象庁、コロナ感染者数データは厚生労働省のものを利用した
  - 気象データ：https://www.data.jma.go.jp/gmd/risk/obsdl/index.php
  - 感染者数データ：https://www.mhlw.go.jp/stf/covid-19/open-data.html

### 分析結果
添付した分析報告書を参照https://github.com/oshipi/corona_weather/blob/main/report.pdf

### 考察
- 線形回帰、ランダムフォレストともに感染者数を精度よく予測することができなかったことから使用する特徴量が適していないか、東京のコロナ感染者数に与える影響には気象要素以外の要因が大きい可能性があると考えられる。
- 年度によって感染者数が大幅に異なることから、コロナウイルスの性質の違いによって感染者数にも変化が表れていると考えられる。
- 予測精度を上げるためには気象とは別の情報（経済状況など）を分析に用いるか、感染したウイルスの性質によってデータを分けるなど、より多くのデータを分析に用いる必要があると考える

### 改善案
以下のような情報があるとより詳細な分析が可能であると考える
- 日ごとの東京の人流データ
- ウイルスの株ごとの感染者数
- 緊急事態宣言や自粛期間中の飲食店の日ごとの売り上げ
- 日ごとのPCR検査の実施状況や実施本数

