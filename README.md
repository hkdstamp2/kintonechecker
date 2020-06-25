# kintonechecker

docker build -t kintonechk:latest .

docker run -it -v `pwd`/app:/app --env-file `pwd`/app/kintonchk.env kintonechk:latest python /app/kintonchk.py



ex)

{{{
start kintone checker
{'text': ':fearful:Everyoneが有効なアプリがありました。\n3:ファイル管理\n更新者:hkd\n閲覧,追加,編集,削除', 'channel': 'ssssss'}
{'text': ':fearful:Everyoneが有効なアプリがありました。\n4:顧客リスト\n更新者:hkd\n閲覧,追加,編集,削除', 'channel': 'ssssss'}
{'text': ':fearful:Everyoneが有効なアプリがありました。\n5:新しいアプリ\n更新者:hkd\n閲覧,追加,編集,削除', 'channel': 'ssssss'}
{'count': 3}

}}}



app/kintonchk.env

set your admin account info

KINTONE_DOMAIN=xxxx.cybozu.com
KINTONE_ID=xxxxx@gmail.com
KINTONE_PASSWORD=xxxxxxx

