## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
https://zipcloud.ibsnet.co.jp/api/search
日本の郵便番号をパラメータとして渡すことで、住所を取得できます。
* リクエストとレスポンスのフォーマット
https://zipcloud.ibsnet.co.jp/api/search?zipcode=1000001

JSON

### Q3-2. 各自で調査したAPIについて説明せよ。
APIの名称と参照URL
Open-Meteo 天気予報API
https://open-meteo.com/
* エンドポイントと機能
https://api.open-meteo.com/v1/forecast
緯度・経度をパラメータとして指定することで、その地点の天気予報データを取得できるサービスです。
* リクエストとレスポンスのフォーマット
https://api.open-meteo.com/v1/forecast?latitude=35.6895&longitude=139.6917¤t_weather=true&daily=temperature_2m_max,temperature_2m_min

JSON

### Q3-3. 感想
* 今回の課題で苦労したこと
APIから返されるJSONデータの構造をconsole.logで確認し、どの階層に目的のデータがあるか確認することが難しかったです。
* 演習を通して理解できたこと
取得したJSONデータをJavaScriptのオブジェクトとして扱い、HTMLに埋め込むDOM操作の技術が分かった。
* Web APIの利便性や課題など
開発者は本来のアプリケーションの機能開発に集中でき、時間を大幅に削減できます。
一方で、APIを提供する外部サービスに完全に依存してしまうと感じました。
