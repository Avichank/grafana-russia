### Установка Grafana 12.0.2 обходным путём

Файл можно скачать напрямую через [Yandex.disk](https://disk.yandex.ru/d/b98pseZJb2yyqw).

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
