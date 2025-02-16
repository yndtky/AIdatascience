学習で書いたPythonのコード、作成した成果物についてここにまとめていきます。
時系列モデルを活用した売上予測を行ないます。

今回はkerasを使って３１アイスクリームの売上高の時系列予測を行ない、予測結果からマーケティング施策の提案を行ってみたいと思います。

この成果物の目的は下記２点です

深層学習フレームワークkerasを使った時系列予測をやってみたかった
予測結果からビジネス視点で何か提案することはできないかと思った
この成果物の流れは次のようになっています。

分析編
①使用データと分析環境
売上データの特徴
作成の流れ
予測結果
分析編の結論
マーケディング編
アプリ会員者数の推移とこれまでの施策
対象にする顧客層
施策提案
工夫点や苦労点など
第一部：分析編

使用データと分析環境

・ここでは31アイスの売上の時系列予測を行なうにあたり、どのようなデータを準備したのかについてまとめます。

・（）の中はデータの取得タイミングと取得元です。

・今回はkerasを勉強するところから始まったことなどもあり、最新の売上予測になっていません。

目的変数：31アイスの売上データ（四半期ごと、31アイスHP）
説明変数：
31Club*の会員者数（四半期ごと、31アイスHP）
東京都の消費支出データ（月ごと、都民のくらしむき（月報）（年報） 内の品目別時系列データ）
東京都の最高気温データ（月ごと、気象庁HP）
データの使用期間：2014年～2023年
環境や分析ツールなど：使用言語Python、深層学習フレームワークkerasを使った時系列予測
※31Clubとは31アイスの会員制アプリのことであり、各種クーポンなど様々なサービスが受けられます。
