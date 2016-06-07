# sample-playbook

## 1. Ansibleのインストール
+ CentoOSの場合  
`$ yum install ansible`

+ OS Xの場合  
`$ brew install ansible`

## 2. hostsファイルの編集
`xx.xx.xx.xx`となっている部分をAnsibleを実行したいサーバーのIPアドレスに変更する

## 3. Ansibleの実行
+ 実行する対象がEC2インスタンスの場合  
`$ ansible-playbook -i hosts site.yml --user=ec2-user --private-key ~/.ssh/xxxx.pem`

## 4. 実行結果の確認
```
$ date
2016年  2月  22日 水曜日 00:00:00 JST
```

サーバー内の時刻合わせ（UTCからJSTへの変更）とyumのupdateができていれば成功です。
