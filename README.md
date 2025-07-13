### Downloads

Файл можно скачать напрямую через [Yandex.disk](https://disk.yandex.ru/d/b98pseZJb2yyqw).

Либо можно установить .deb командой ниже

```bash
wget "https://s759sas.storage.yandex.net/rdisk/7fff0317783d51ddae9afd9442200955d761606b2d1051285270718a1da617fe/6873c8b4/jCsUHhQ3ANDObRWMmUxX3qBsPYOvkdlXXOrKiMpffWZgEwAoXrJCQe6jKDNunPPfLwzQ9o1quU0093iUrOxzdw==?uid=0&filename=grafana-enterprise_12.0.2_amd64.deb&disposition=attachment&hash=c79STZBL+X8RJscgkDPxe3SS0kA67+J5/WIHS6TtG7ZM6VlodZQczwkv3sAY4CI/q/J6bpmRyOJonT3VoXnDag==&limit=0&content_type=application/vnd.debian.binary-package&owner_uid=255445559&fsize=182404332&hid=e069cfa75616bb4ed71bb1d019ac97b3&media_type=compressed&tknv=v3&ts=639d0b93c9500&s=5c1b1999addd4a710c94f659ee04608d55fe862ef1c38a371c78bbc272a4a94a&pb=U2FsdGVkX1-xTvD0Ule9igddLqLm9avCgj7xrR06VWhTFgiq4-WXVtitDlkZ_SE3fuz0KjQtPXwpDJBC98ovfs6ixSIq_Fz1mWCL1i8CETg" -O grafana_12.0.2.deb
```
Затем нужно запустить установку 

```bash
sudo dpkg -i grafana_12.0.2.deb
```

Теперь активизуем и запустим сервис

```bash
sudo systemctl daemon-reload
sudo systemctl enable grafana-server
sudo systemctl start grafana-server
```

Готово! Теперь по адресу localhost:3000 доступен интерфейс Grafana. Вход по умолчанию admin:admin

Prometheus will now be reachable at <http://localhost:9090/>.
