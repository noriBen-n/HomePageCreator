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

## 現在使用している写真（5件）

Wikimedia Commonsで公開されている、クリエイティブ・コモンズ・ライセンス（CC BY / CC BY-SA）の写真を使用しています。

| 施設 | ファイル | 撮影者 | ライセンス |
|---|---|---|---|
| 大阪城（id:2） | osaka-castle.jpg | Onyo | CC BY-SA 4.0 |
| 梅田スカイビル（id:4） | umeda-sky-building.jpg | Kakidai | CC BY-SA 4.0 |
| 通天閣（id:17） | tsutenkaku.jpg | Fabio Achilli | CC BY 2.0 |
| 住吉大社（id:54） | sumiyoshi-taisha.jpg | Hyppolyte de Saint-Rambert | CC BY 4.0 |
| 仁徳天皇陵古墳（id:65） | nintoku-kofun.jpg | 国土地理院 | カラー空中写真（要出典表記） |

これらのライセンスは**クレジット表記が必須**なので、`index.html` フッターの「写真クレジット」欄に記載しています。他にWikimedia Commonsなどからライセンス写真を追加する場合は、同様にここへクレジットを追記してください（自分で撮影した写真であれば、クレジット表記は不要です）。
