# Домашнее задание к занятию "10.01. Зачем и что нужно мониторить"

1.
- Метрики дисковых операций ввода-вывода, пропускной способности и длины очереди. т.к. отчеты сохраняются на диск
- Метрика загруженности процессора. т.к. вычисления загружают ЦПУ
- Метрики кодов ответов http т.к. взаимодействие идет по протоколу http
2. Надо выяснить какие обещания даны клиентам это будет SLA, после чего поставить цели соответствующие этим обещаниям это будет SLO. и подобрать метрики которые будут показывать уровень соответствия сервиса с целями эти метрики будут SLI
3. Использовать например elastalert поверх ELK и трассировку стеков
4. Думаю это из-за кодов 3хх, правильнее так: (summ_2xx_requests + summ_3xx_requests)/summ_all_requests хотя некторые 4хх тоже можно поднять наверх как мне кажется например 403, 451
