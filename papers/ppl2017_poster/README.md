## 著者名

岡部 究

## 所属

理化学研究所 計算科学研究機構

# 1. 発表タイトル: (ポスター・デモ)

C言語ヘッダからのATS言語関数シグニチャの自動生成と段階的な線形型の導入

## キーワード(3つ以上)

コード自動生成
低レベルプログラミング
線形型
リソースリーク

## 発表概要(200〜300字程度)

C言語を用いた低レベルなプログラミングにおいてメモリ破壊やリソースリークはやっかいな問題です。C言語の代替としてATS言語 http://www.ats-lang.org を採用し、線形型を用いてメモリアクセス権限やリソース生存範囲を表明することで、これらの違反をコンパイル時検査できることが知られています。しかし既存のC言語コード資産の上でATS言語実装を動かすには、当該C言語関数をATS言語にインポートする必要がありました。本論文では、この人為的なミスを誘発するプロセスをコード生成によって自動化する https://github.com/metasepi/c2ats というツールを提案します。

# 2. 発表タイトル: (ポスター・デモ)

RTOSシステム状態の静的検証手法から見たATS言語とVeriFast検証器の比較

## キーワード(3つ以上)

RTOS
線形型
プログラム検証ツール
シンボリック実行

## 発表概要(200〜300字程度)

RTOSの1つである http://www.chibios.org は独自のシステム状態を持っています。このRTOSは実行中にAPI呼び出しや割り込みによってこのシステム状態を遷移させながら動作します。現在のシステム状態から当該システム状態に対応していないAPIを呼び出した場合にはアプリケーションの実行時に未定義のエラーが発生します。このような実行時エラーをまねく不変条件をコンパイル時に検査するために http://www.ats-lang.org を用いることができることを示します。また同じ検査をプログラム検証ツールであるVeriFast https://github.com/verifast/verifast も用いることができることも示します。