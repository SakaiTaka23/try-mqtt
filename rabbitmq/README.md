# rabbitmq

- Dockerイメージについて managementというものが入ったイメージは管理コンソールが入っている
- mqttのプラグインを有効化すること
```shell
rabbitmq-plugins enable rabbitmq_mqtt
```

## publish
mosquitto_pub -h host.docker.internal -p 15672 -d -t hello_topic -m "hello"

## subscribe
mosquitto_sub -h host.docker.internal -p 15672 -d -t hello_topic


# 役割
- broker → broker
- client1 → publisher
- client2 → subscriber
