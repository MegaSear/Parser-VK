--------------------------------------------------------------------------------------------

Этот код собирает сохранённые данные логинов и паролей и использует для авторизации в ВК.
 Далее, берёт headers и cookies из драйвера selenium для POST запросов.
 Далее, обработка response как json объект и извлечение необходимых данных.
 Далее, композиция данных в data frame и сохранение в папке.
 Данные - все сообщения каждого чата юзера.
    
Описание полученных data frame:
  В папке Archive_'user_id' хранятся csv-файлы в формате:
  Status_Chat + Id_Chat + .csv
  Где Status_Chat может быть Pesonaly или Group в зависимости от типа чата (личка, беседа)
  Id_Chat - id чата 
  В самом файле содержатся информация сообщений чата. (Id отправителя, текст, время)

--------------------------------------------------------------------------------------------
P.S.
vk api не используется

P.P.S
Перед использованием парсера не забудьте сохранить свой пароль вк в браузере Chrome.
