# 概要

#### Dockerイメージ（GitLab）

    Docker 環境で GitLab を起動します。Windows 環境でも動作します。

#### 動作環境

    Docker 環境で実行します。Windows 環境でも動作します。

# 利用方法

#### Docker-Compose で起動

    - 1.「docker-compose.yml」格納ディレクトリに移動
        $ cd 【格納ディレクトリ】

    - 2.コンテナ起動
        $ docker-compose up
        ※完全に起動するまでに、10～15分ほど要する

    - 3.動作確認
        ブラウザから接続（起動中は 502 ERROR）
            ・http://192.168.99.100/
        
        補足）初回起動時にrootのパスワード変更を行いログインする
        補足）ログイン後、「Settings」の「Preferences」の「Language」を「日本語」
              にすることでメニューが日本語になる
        補足）別コンソールでコンテナに接続
        $ docker exec -it  gitlab /bin/bash

    - 4.コンテナ停止
        ・[Ctrl]+[C] または $ docker-compose stop

    - 5.コンテナ削除
        $ docker-compose rm -f

    - 6.イメージ削除
        $ docker system prune -a
