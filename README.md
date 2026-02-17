# Linux-useful-commands
Linuxの便利なコマンド

- 文字列検索



    ~~~

    grep -r -nr "string" ./*

    ~~~



- ファイル名検索



    ~~~

    # stringに検索したいファイル・フォルダー名の一部を設定

    find -name "*string*"



    # 例：imageを含むファイル・フォルダーを検索する場合

    find -name "*image*"



    # 例：image_folderを検索する場合

    find -name "image_folder"

    ~~~



- 動画から静止画



    ~~~

    # <frame_num>に切り出す時刻を設定

    ffmpeg -ss <frame_num> -i input.mp4 -frames:v 1 frame.png



    # 例：10フレーム目を切り出す

    ffmpeg -ss 10 -i input.mp4 -frames:v 1 frame.png

    ~~~



- クローンしたリポジトリのSHA(バージョン)確認



    ~~~

    git show --format='%H' --no-patch

    ~~~



- クローンしたリポジトリのSHA(バージョン)変更



    ~~~

    cd <repository>

    git checkout <SHA>

    ~~~
