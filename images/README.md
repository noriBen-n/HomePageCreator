# 施設写真の追加方法

このフォルダに施設の写真を置くと、トップページのイラストの代わりに実写真が表示されます。

## 手順

1. **自分で撮った写真、または利用許諾のある写真だけ**をこのフォルダに追加してください（施設の公式サイトやGoogle Mapから無断で写真を持ってくるのはNGです）
2. ファイル名は分かりやすいものに（例: `kaiyukan.jpg`、`usj-01.jpg`）
3. `index.html` 内の `<script>` の中にある `PHOTOS` という一覧に、施設のIDとファイルパスを追加します

```js
var PHOTOS = {
  3: "images/kaiyukan.jpg",
  6: "images/harukas300.jpg",
};
```

施設のIDは `venuesData` の中の `"id"` の値です（`id:3` は海遊館、`id:6` はハルカス300、など）。

## 推奨サイズ

- 横長（例: 800×450px 程度）
- ファイルサイズは1枚あたり300KB以下を目安に（表示速度のため）
- JPG形式を推奨

`PHOTOS` に追加していない施設は、これまで通りイラストのまま表示されます。

## 現在使用している写真（29件）

Wikimedia Commonsで公開されている、クリエイティブ・コモンズ・ライセンス（CC BY / CC BY-SA）の写真を使用しています。

| 施設 | ファイル | 撮影者 | ライセンス |
|---|---|---|---|
| 大阪城（id:2） | osaka-castle.jpg | Onyo | CC BY-SA 4.0 |
| 海遊館（id:3） | kaiyukan.jpg | そらみみ | CC BY-SA 4.0 |
| 梅田スカイビル（id:4） | umeda-sky-building.jpg | Kakidai | CC BY-SA 4.0 |
| あべのハルカス（id:6） | abeno-harukas.jpg | Oilstreet | CC BY-SA 3.0 |
| なんばグランド花月（id:7） | ngk.jpg | MASA | CC BY-SA 3.0 |
| 心斎橋筋商店街（id:18） | shinsaibashi-suji.jpg | Mc681 | CC BY-SA 4.0 |
| 黒門市場（id:19） | kuromon-ichiba.jpg | Mc681 | CC BY-SA 4.0 |
| さきしまコスモタワー展望台（id:20） | cosmo-tower.jpg | Kirakirameister | CC BY-SA 3.0 |
| 天王寺動物園（id:22） | tennoji-zoo.jpg | Wing1990hk | CC BY 3.0 |
| グラングリーン大阪 うめきた公園（id:26） | grand-green-osaka.jpg | Tokumeigakarinoaoshima | CC BY-SA 4.0 |
| 国立民族学博物館（id:32） | minpaku.jpg | Fk | CC BY-SA 2.5 |
| 大阪市立科学館（id:36） | osaka-science-museum.jpg | MASA | CC BY-SA 3.0 |
| 国立国際美術館（id:37） | national-museum-art.jpg | Mc681 | CC BY-SA 4.0 |
| 大阪市立東洋陶磁美術館（id:39） | oriental-ceramics-museum.jpg | Oilstreet | CC BY-SA 3.0 |
| 天保山大観覧車（id:12） | tempozan-ferris-wheel.jpg | 663highland | CC BY-SA 3.0 |
| 通天閣（id:17） | tsutenkaku.jpg | Fabio Achilli | CC BY 2.0 |
| 中之島公園バラ園（id:40） | nakanoshima-rose-garden.jpg | Laitche | CC BY-SA 4.0 |
| 大阪天満宮（id:42） | osaka-tenmangu.jpg | 663highland | CC BY-SA 3.0 |
| 大阪歴史博物館（id:45） | osaka-museum-history.jpg | Onyo | CC BY-SA 4.0 |
| 難波八阪神社（id:47） | namba-yasaka-shrine.jpg | Immanuelle | CC BY 4.0 |
| 四天王寺（id:51） | shitennoji.jpg | そらみみ | CC BY-SA 3.0 |
| 長居公園（id:53） | nagai-park.jpg | Naokijp | CC BY-SA 4.0 |
| 住吉大社（id:54） | sumiyoshi-taisha.jpg | Hyppolyte de Saint-Rambert | CC BY 4.0 |
| 服部緑地公園（id:56） | hattori-ryokuchi.jpg | 663highland | CC BY-SA 3.0 |
| 岸和田城（id:59） | kishiwada-castle.jpg | 663highland | CC BY-SA 3.0 |
| 箕面公園・箕面大滝（id:62） | minoo-falls.jpg | 663highland | CC BY-SA 3.0 |
| 浜寺公園（id:64） | hamadera-park.jpg | Midori | CC BY-SA 3.0 |
| 仁徳天皇陵古墳（id:65） | nintoku-kofun.jpg | 国土地理院 | カラー空中写真（要出典表記） |
| 大仙公園（id:66） | daisen-park.jpg | Laitche | CC BY-SA 4.0 |

これらのライセンスは**クレジット表記が必須**なので、`index.html` フッターの「写真クレジット」欄に記載しています。他にWikimedia Commonsなどからライセンス写真を追加する場合は、同様にここへクレジットを追記してください（自分で撮影した写真であれば、クレジット表記は不要です）。
