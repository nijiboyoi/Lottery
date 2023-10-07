# Lottery

くじアプリ仕様書
1. ページ構造
HTMLファイルで構築されており、各くじは<div>要素で表現されている。
各くじにはID（omikuji1からomikuji9）が振られている。
2. スタイリング
各くじは.omikujiクラスを持ち、ボーダー、パディング、マージンなどの基本的なスタイリングが適用されている。
スタイリングは変更可能で、ユーザーが好みに合わせて調整できる。
3. くじの結果表示
各くじには？が含まれており、初期状態では不明な結果（"？"）が表示されている。
4. JavaScriptによるくじ引き
drawOmikuji 関数が実装されており、各くじをクリックすることでくじを引くことができる。
当たりの確率は現在10%で、ランダムに当たりかハズレが決定され、結果が表示される。
5. イベントリスナー
各くじに対して、クリックイベントがリスナーとして設定されており、クリックされた時に drawOmikuji 関数が呼び出される。
