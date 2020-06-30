# RLResources

強化学習に関する論文や実装等に関する情報


## RSS フィード

Slack に RSS アプリをインストールして, `/feed subscribe [フィードのアドレス]` とすると定期的に論文情報を取得.


### arXiv API (Reinforcement Learning)

[arXiv API](https://arxiv.org/help/api) で "reinforcement learning" を全フィールド (all) で検索して投稿日 (submittedDate) でソートして20件取得.

https://export.arxiv.org/api/query?search_query=all:%22reinforcement%20learning%22&sortBy=submittedDate&sortOrder=descending&max_results=20

上記 arXiv API の結果を Feed43 で加工してサムネイル画像等が出るようにしたもの. ただし, 論文が新しすぎてサムネイル等の生成が間に合っていないことが多い. 最初の著者しか取得出来ていない.

https://feed43.com/arxiv_api_rl.xml


### arXivTimes

[arXivTimes](https://github.com/arXivTimes/arXivTimes) の[論文の一言まとめ](https://github.com/arXivTimes/arXivTimes/issues). GitHub の issues には RSS が対応していないようなので Feed43 で RSS 生成. 最新の5件しか取得出来ていない. アルファベット順で最初のカテゴリしか取得出来ていない. issues 本文が取得出来ていない(Slack がリンクから展開して前半部分だけ表示はしてくれる).

https://feed43.com/arxivtimes.xml


### Arxiv Sanity Preserver (top hype)

[Arxiv Sanity Preserver](http://www.arxiv-sanity.com/) の [top hype](http://www.arxiv-sanity.com/toptwtr). Twitter でメンションされた論文(直近1日)の上位15件程度. 1, 2 回しかメンションされていない場合でも表示される場合があるので若干ノイズ多め. 本当は直近1週間の結果を表示したいが Feed43 の制限(無料版は100KBまで)で無理だった.

https://feed43.com/arxiv_sanity_top_hype.xml


### Arxiv Sanity Preserver (top recent, last week)

[Arxiv Sanity Preserver](http://www.arxiv-sanity.com/) の [top recent](http://www.arxiv-sanity.com/top). ライブラリに保存された論文(直近1週間)の上位20件.

https://feed43.com/arxiv_sanity_top_recent.xml
