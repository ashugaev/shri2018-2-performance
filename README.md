# Порядок дейсвий для оптимизации загрузки

1. Сжал все изображения (качество и размер) и png перевел в jpeg
2. Изображения до 2х кб заинлайнил в css
3. Фавикон тоже сжал и закинул в base64
4. Убрал бабель и реакт. Убрал рендер компонента через реакт.
5. Убрал бутстрап и шрифты вынес в index.html. Так же сказал только нужные варианты шрифта в формате woff2
6. Убрал лишние 25 000 строк яваскрипта не влияющие на функционал и поставил асинхронную загрузку для файла
7. Убрал файл banner.js , которые рендерит баннер. Вынес html наружу.
8. Выкинул комменты из html
9. Минифицировал js и css. html не стал, что бы был виден дифф в пуллреквесте.

Я не все изменения заливал на проверку, потому что на 1 проверку уходит около 10 минут, я тратил 2 часа, что бы понять что не нравится сервису или пока искал качество картинки на которое он не будет ругаться. В общем это классно, но слишком долго.
