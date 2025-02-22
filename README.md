
# UplinkOS_RUS

Работа над локализацией игры периодически ведется с 2006 года в качестве хобби одим человеком.
За это время проект дважды менял инструментарий и вектор развития, однажды откатывался из за потери данных. Затем, был создан этот репозиторий.


### Состояние проекта на 2021 год: 

**Просто поиграть:**
Версия в [инсталляторе](http://uplinkos.ru/) стабильна и  вполне играбельна. При моих тестах за последние 100 часов игры не случилось ни одного вылета. Переведена бóльшая часть игры.

Для прохождения рекомендую эту версию.

**Хочу помочь:**
Если тебе не лень разбираться и ты готов к встрече с багами, в этом репозитории ты можешь [скачать](https://github.com/kesha4/UplinkOS_rus/archive/master.zip) мой промежуточный билд. Он немного свежее версии в инсталляторе и в нем возможны шероховатости. Увидишь что-то странное - сделай скриншот и напиши мне в телегу. Контакты в самом низу страницы. Тестер по желанию увековечивается в укромном месте внутри локализации игры.

Принято правок от тестеров: 4.

При прохождении игры не желательно обновляться, т.к. сейвы могут работать некорректно.

**Хочу научиться:**
Маякни мне если хочешь освоить ремесло кустарного перевода программ. Оно забывается, а я с радостью научу, но мне нужно понять интересно ли это кому-то. Работу над видео начну когда наберется фокус-группа из 10 желающих его посмотреть. 

Маякнули: 1 человек.





### Установка:

С сентября 2020 года выпускается инсталлятор *(https://kesha4.github.io/UplinkOS_rus/)*

Работает на версии Uplink от магазина GOG (и возможно на старой дисковой версии). **Не работает на версии от Steam!**

После установки локализации ОБЯЗАТЕЛЬНО нужно начинать новую игру. В старых сохранениях перевод не применится.


### Что уже переведено:
1. Заменен основной шрифт.
2. Главное меню.
3. Настройки.
4. Интро нового пользователя.
5. Начальный интерфейс (HUD).
6. Туториал.
7. Ссылки в InterNIC.
8. Не уникальные новости о взломах корпораций.
9. Новости о взломе Сoциальной БД.
10. Новости о взломе Академической БД.
11. Новости о взломе Криминальной БД.
12. Новости о взломе систем с разрушением сервера.
13. Новости о взломе с большим объемом данных.
14. Новости об арестах.
15. 5 уникальных новостей.
16. 12 уникальных писем.
17. Описания программ в магазине.
18. Описания железа в магазине.
19. Описания шлюзов в магазине.
20. Перевод консоли (~50%).
21. Задания ур. 1-5.
22. Письма для соответствующих заданий.
23. Окно чата с заказчиком.
24. Логи.
25. Государственные базы данных.
26. Разделы справки (все).
27. Звания рейтинга Нейромансер.

99 . Продолжение списка в описании коммитов.  

### Чего не стоит ждать в ближайшее время:
1. Возможности печатать на русской раскладке. Оставил попытки и добавил вписывающееся в лор пояснение в игре.
2. Названия корпораций, имена людей, псевдонимы хакеров. Проблемы с поиском, см. п. 1.
3. Голоса для голосового анализатора. Нет оборудования и специалиста обработки звука. Смысла в этом тоже нет.
4. UplinkOS_RUS для Steam версии игры. Локализация будет портирована и на нее позже. Сейчас можно купить [GOG версию](https://www.gog.com/game/uplink_hacker_elite) за 3$ или поставить UplinkOS_RUS на [пиратку](https://g.zeos.in/?q=Uplink%20ENG%20GOG%20%D1%81%D0%BA%D0%B0%D1%87%D0%B0%D1%82%D1%8C%20%D0%B1%D0%B5%D1%81%D0%BF%D0%BB%D0%B0%D1%82%D0%BD%D0%BE).

### Предыстория:
За локализацию я взялся т.к. в детстве играл в оригинальную игру в пиратском переводе под названием **"Сеть"**, но из за ошибок перевода она была непроходима. 
Модификация графики **"[Uplink OS](https://www.moddb.com/mods/uplink-os)"** получилась шикарной, рекомендую всем фанатам оригинальной игры ознакомиться с ней. Очень жаль, что *[Cpt.McBacon](https://www.moddb.com/members/cptmcbacon)* и *[JesseTG](https://www.moddb.com/members/jessetg)* прекратили разработку на версии GOLD. Насколько я могу судить, она местами сыровата. Кроме того, авторы модификации собирались сделать возможность простой локализации через XML файлы, но забросили реализацию этой фичи на полпути. В результате мы имеем часть строк жестко закодированных в EXE, а часть - в XML ресурсах игры. 

#### Инструментарий
Я пытался связаться с командой разработчиков **"Uplink OS"** для помощи им в разработке и локализации стандартными средствами, но тщетно. Они не отвечают и больше не занимаются проектом. В связи с этим было принято решение локализовать **"UplinkOS"** доступными мне инструментами. Итак, чем я пользуюсь:

* **Radialix** - используется для перевода жестко закодированных *ASCII* строк в файле *UplinkOS.exe*
* **IDA** - дизассемблер с которым работает *Radialix* для поиска ссылок на жестко закодированные строки
* **Notepad++** - для перевода части строк вынесенных в XML файлы 
* **Translate my UTF8-HEX** - созданный мной скрипт для удобного перевода UTF8 строк *(см. сложности перевода)*

#### Сложности перевода
Перевод через программу *Radialix* это фактически более удобная форма редактирования исполняемого файла в HEX-редакторе, где нельзя выходить за рамки отведенного каждой строке места внутри файла. Т.к. при программировании авторы модификации использовали кодировку UTF8 (в ней кириллические символы занимают в 2 раза больше байт чем латинские), то все переводимые жестко закодированные строки приходится сжимать в 2 раза. Чтобы хоть как-то обойти эту особенность, мной был написан скрипт *Translate my UTF8-HEX*, который автоматически подставляет вместо кириллических букв похожие латинские (А/A, и/u, ь/b, и тд.). А также подсказывает, на сколько байт следует сократить перевод чтобы он влез в отведенное для строки место. 

~~Именно по этой причине я не перевожу многие короткие слова (обычно и без перевода понятные). Например слово **No** занимает всего 2 байта, а слово **Нет** уже все 6 байт (4 при обработке скриптом).~~

Короткие часто встречающиеся слова переводятся и обрабатываются как отдельный шрифт (каждый символ этого фрифта выглядит как слово или иконка).

Фразы вводимые с клавиатуры оставлены без перевода в угоду проходимости игры, т.к. возможность менять раскладку клавиатуры в UplinkOS не предусмотрена.

### Лицензия
##### Лицензия перевода
Этот перевод является свободным программным обеспечением. Вы можете распространять и/или модифицировать его с сохранением указания автора проекта (**Сергей _"kesha4"_ Макаров**). Не рекомендуется использовать данный перевод и его производные для получения денежной выгоды. 
Этот перевод распространяется в надежде, что он будет полезен, но БЕЗ ВСЯКИХ ГАРАНТИЙ, в том числе подразумеваемых гарантий ТОВАРНОГО СОСТОЯНИЯ ПРИ ПРОДАЖЕ и ГОДНОСТИ ДЛЯ ОПРЕДЕЛЁННОГО ПРИМЕНЕНИЯ. Автор не несет никакой ответственности в случае неполадок вызванных данным продуктом, а также в случае возникновения острого психоза на фоне неточности перевода.
##### Лицензия Uplink
Данный репозиторий содержит оригинальные файлы игры [**Uplink: Hacker Elite** с сайта _GOG.com_](https://www.gog.com/game/uplink_hacker_elite), которые приложены для примера. Удалите их, если вы не покупали игру на указанном сайте. Оригинальные файлы игры содержатся в самом первом коммите. Все права принадлежат разработчику **Introversion Software**. Подробнее см. файл *readme.txt*.
##### Лицензия UplinkOS
Данный репозиторий содержит также оригинальные файлы модификации **[Uplink OS](https://www.moddb.com/mods/uplink-os)** за авторством **[Cpt.McBacon](https://www.moddb.com/members/cptmcbacon)** и **[JesseTG](https://www.moddb.com/members/jessetg)**, все права принадлежат им. Оригинальные файлы модификации содержатся во втором коммите. Подробнее см. файл *UplinkOS_ReadMe.txt*. 

### Контакты

- [Сайт проекта: UplinkOS.RU](http://uplinkos.ru/)
- [Telegram: @uplinkos_rus](https://t.me/uplinkos_rus)
- [YouTube:  UplinkOS RUS](https://www.youtube.com/channel/UCLytGPWNGLMDv7xXlpafj8A)
- [E-mail: kesha4elovek@gmail.com](mailto:kesha4elovek@gmail.com)

### Ссылки связанные с проектом:
- [Uplink: Hacker Elite –  GOG.com](https://www.gog.com/game/uplink_hacker_elite)
- [Uplink OS modification (GOLD GOG version)](https://www.moddb.com/mods/uplink-os)
- [Uplink  – Wikipedia](https://ru.wikipedia.org/wiki/Uplink)
