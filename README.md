# Простое приложение для проверки работы службы RabbitMQ

## Установка RabbitMQ (Debian-Way)
$ sudo apt install rabbitmq-server
$ sudo rabbitmq-plugins enable rabbitmq_management

# Установка зависимостей, запуск
1. go get github.com/rabbitmq/amqp091-go
2. go run rabbit-checker.go

Ожидаемый вывод:
```
$ go run rabbit-checker.go
2022/07/15 11:42:36  [x] Sent rabbit-checker
2022/07/15 11:42:36  [*] Waiting for messages. To exit press CTRL+C
2022/07/15 11:42:36 Received a message: rabbit-checker
```