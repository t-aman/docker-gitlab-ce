
【修正中】

# 概要

#### Dockerイメージ（GitLab）

    Docker-ComposeでGitLab環境を生成します。

#### 動作環境

    Docker環境で実行します。

# 利用方法

#### Docker-Compose で起動

    - 1.「docker-compose.yml」格納ディレクトリに移動
        $ cd 【格納ディレクトリ】
        
        例）
        $ cd d:/WORK/docker-lamp
    
    - 2.コンテナ起動
        $ docker-compose up -d

    - 3.動作確認
        ブラウザから接続
            ・http://192.168.99.100/
        
        補足）サーバのIPアドレスはDockerで確認
        $ docker-machine ip

    - 4.コンテナ停止・削除
        $ docker-compose stop
        $ docker-compose rm -f
