# UDP加密聊天室

## 功能

- [x] UDP协议通信
- [x] Json格式通信
- [x] AES-256加密通信
- [x] 客户端/服务器读取本地配置文件
- [x] 密钥随机生成


# 语言

* Golang ![golang](http://i.imgur.com/UEdZpr4.png)

## 客户端

配置文件位于`~\chat-config.json`

例子
```json
{
	"listen": ":52915",
	"remote": "127.0.0.1",
	"key": "AzonXhdbWCYoAA52GTE9FnldZEN4KhEsInFJe1oHYAgzQTRsCyEdUlBOPzd3HxgFbTAudDZobiU8TQYbURBFWVdvMisNSn5UIw8kei0gcjl1cGkeFTV9U0tEY2YaCkdPYl9nZRQSBGsMQgFzVlxhL0hGAlV/O0A+OGoJfBwpE0w="
}
```
启动客户端后需要配置用户id和昵称

``
./client
``

## 服务端

配置文件位于`~\chat-config.json`

例子
```json
{
	"listen": ":52915",
	"remote": "", //随意可不填
	"key": "AzonXhdbWCYoAA52GTE9FnldZEN4KhEsInFJe1oHYAgzQTRsCyEdUlBOPzd3HxgFbTAudDZobiU8TQYbURBFWVdvMisNSn5UIw8kei0gcjl1cGkeFTV9U0tEY2YaCkdPYl9nZRQSBGsMQgFzVlxhL0hGAlV/O0A+OGoJfBwpE0w="
}
```

``
./server
``


## 参考

[https://github.com/digitalis-io/golang-udp-chat](https://github.com/digitalis-io/golang-udp-chat)

[https://github.com/gwuhaolin/lightsocks](https://github.com/gwuhaolin/lightsocks)
