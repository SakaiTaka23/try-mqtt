# mosquitto

## publish
mosquitto_pub -h host.docker.internal -p 1883 -d -t hello_topic -m "hello"

## subscribe
mosquitto_sub -h host.docker.internal -p 1883 -d -t hello_topic


# 役割
- broker → broker
- client1 → publisher
- client2 → subscriber


## TODO
pahoのgoでパブサブをしてデータの操作ができることを確認する

main.goを実行することによって呼び出せることを確認できた
