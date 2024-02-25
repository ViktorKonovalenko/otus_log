# otus_log
Для выполнения ДЗ используется vagrant  в паре с Ansible. После запуска vagrant файла создается две виртуальные машины настроенные с помощью Ansible согласно методичке.<br>
Запускаем vagrant 
<pre>vagrant up</pre>
Подключаемся к web
<pre>vagrant ssh web</pre>
Проверяем работу логирования ошибок nginx согласно методичке<br>
![image](https://github.com/ViktorKonovalenko/otus_log/assets/32430041/991b9405-b287-450d-aa26-edc116e484a3)
Проверяем работу логирования access nginx согласно методичке<br>
![image](https://github.com/ViktorKonovalenko/otus_log/assets/32430041/e30f6ed2-9aad-4992-b232-f1c28efd0ac4)
Проверяем работу аудита изменения конфигурации nginx согласно методичке<br>
![image](https://github.com/ViktorKonovalenko/otus_log/assets/32430041/6bb1ccdf-80b4-4747-97f3-db6c5ceb0183)
