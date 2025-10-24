# BOOTHの商品ページのJSONスキーマ

## description

自由記述の文字列。プレーンテキスト。
改行は `\n` として表現される。

## id

商品のID。数値。

## is_adult

R-18かどうか？

## is_end_of_sale

発売停止したかどうか？

## name

商品のタイトル

## published_at

商品が公開された日時。ISO 8601形式。

## wish_lists_count

いいねしたユーザーの数？

## category

### id

サブカテゴリに対するカテゴリID？

### name

サブカテゴリの名前

### parent

#### name

カテゴリの名前

#### url

カテゴリに該当する商品を絞り込むための検索用URL

### url

サブカテゴリに該当する商品を絞り込むためのURL

## embeds

### (item)

HTML。YouTubeなどの埋め込み？

## images

### (item)

#### caption

(undocumented)

#### original

原寸サイズの画像

#### resized

リサイズされた画像

### order

リクエストを送信したアカウントが購入していれば、以下のオブジェクト
購入していなければnull

#### purchased_at

YYYY年M月D日

#### url

`https://accounts.booth.pm/orders/{order_id}`

### gift

リクエストを送信したアカウントでギフトを受け取っていれば、以下のオブジェクト
購入していなければnull

