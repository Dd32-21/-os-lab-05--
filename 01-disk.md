В шаге первом нужен вывод команды  lsblk /dev/loop0 , прилагаю скриншот 

<img width="536" height="126" alt="image" src="https://github.com/user-attachments/assets/0efaaa82-e70a-4c52-8c8c-c6dbca3ef3db" />

Далее прилагаю скриншот вывода blkid

<img width="1571" height="125" alt="image" src="https://github.com/user-attachments/assets/c5e7b8ec-d161-43e2-a0cf-727ac4644f2f" />

Здесь нам показан UUID каждого, а также его тип 

Далее прилагаю скриншот вывода команды  df -hT Подробно описал проблему в что о пошло не так 

<img width="702" height="114" alt="image" src="https://github.com/user-attachments/assets/e8fe947d-d7c4-4d64-8867-ad29439841e9" />

Я думаю что раздел ext4 занят сразу потому что те самые  структуры как журнал и служебные файлы автоматически заносятся при монтировании диска и поэтому чуть чуть места занято 
