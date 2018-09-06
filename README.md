# MINIOをサービス化する用の設定ファイル　※Azure用に設定

1.起動用の専用ユーザーを作成

sudo useradd -s /sbin/nologin minio-user

2.minio.service を下記のディレクトリに配置

/etc/systemd/system/minio.service

3.minio.conf を下記のディレクトリに配置

/etc/default/minio.conf

4.サービスの有効化

sudo systemctl enable minio

5.サービスの起動

sudo systemctl start minio

※参考サイト

https://qiita.com/uehatsu/items/1c00a84347c867b99ea0
