Команда ls -li прилагаю скриншот, то что она выдала 

<img width="767" height="155" alt="image" src="https://github.com/user-attachments/assets/ffc82f91-7b28-4c5c-88bd-766328c16048" />

orig и hard имеет одинаковые inode 13 которая имеет 2 ссылки 

Вводим cat hard.txt и нам выдает 

<img width="498" height="45" alt="image" src="https://github.com/user-attachments/assets/7728812c-fe83-4f9d-b0fc-28fa62ca750f" />

Далее echo и вводим cat soft.txt и нам выдает 

<img width="528" height="46" alt="image" src="https://github.com/user-attachments/assets/616f4ed7-ba8d-498e-ab6e-928cbac0a2db" />

Это означает что символическая ссылка не пережила удаление 
Жесткая ссылка пережила удаление, потому что это сам файл, а символическая всего лишь ярлык
Я считаю, что жёсткую ссылку нельзя сделать на файл с другого раздела, потому что inode уникален внутри одного раздела. 
