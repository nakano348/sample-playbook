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
