# JavaScript Flashcards (флэш – карты JavaScript)

## Введение
Мы собираемся создать приложение для флэш-карт, которое работает в точности как приложение, показанное на Рисунке 1, однако нет необходимости создавать его точную копию. У нас другая задача – сосредоточиться на написании элегантного, объектно-ориентированного кода, не забывая при этом о дизайнерских решениях и об отборе лучших методов действий.

![flashcards animation](readme-assets/flashcards-animation.gif)
*Рисунок 1*. Пример реализации флэш-карты.


### Model-View-Controller
Мы собираемся разработать наш код таким образом, чтобы следовать Model-View-Controller [Model-View-Controller][wikipedia mvc] (MVC)[шаблон дизайна][шаблон дизайна Википедия]. Прежде чем мы начнем выполнять releases, нужно убедиться в том, что мы можем ответить на следующие вопросы.

- Что представляет собой Model?
- Как используется View?
- В чем заключаются обязанности Controller?


## Releases
### Pre-release: описание и дизайн приложения
Прежде чем мы начнем писать наш код, давайте договоримся о том, как мы будем выстраивать наше приложение. Как выглядит наша игра с колодой флэш -карт – от момента загрузки данных в файл до проверки того, верна ли наша догадка? Что должно происходить? Как было указано во *Введении*, наше приложение должно работать так, как было показано на Рисунке 1, но не обязательно должно быть его точной копией:   например, мы можем дать пользователям не одну, а несколько попыток  для того, чтобы отгадать карточку.

Когда у нас сформируется четкое понимание того, что должно происходить, тогда можно приступать к разработке проекта приложения. Мы должны иметь возможность нарисовать или написать черновой вариант объектов, которые мы собираемся получить (т. е. наши модели данных), их взаимодействие между собой, а также общий поток (ход) нашей программы.

Этот release занимает приблизительно 15-20 минут. Если это займет больше времени, и вы почувствовали, что застряли, то найдите человека, который поможет вам справиться с возникшей проблемой.

### Release 0: Построение шаблона Model-View-Controller

Когда мы находимся на странице, связанной с выбором дизайна для нашего карточного приложения, мы начинаем заниматься его построения. У нас есть несколько примеров файлов данных (например, `nighthawk_flashcard_data.txt`), и пользователь должен иметь возможность воспроизвести любой из этих файлов.

При выполнении задания, следуйте как можно точнее шаблону проектирования MVC. Наш  нынешная реализация, скорее всего, будет отличаться от нашей реализации его когортных товарищей, и это нормально. Важно понимать, насколько хорошо мы структурируем наш код для представления абстрактной концепции шаблона проектирования.

*Примечание:* Здесь представлен[пример реализации MVC][mvc-hospital-example.md] для приложения, связанного с больницей.

## Заключение
Подумайте о решениях, которые мы принимали во время выполнении этой задачи. Каковы были результаты от дизайнерских решений, принятых нами в *Pre-release*, когда мы только начали разрабатывать наше приложение? Упростили ли они нашу работу по шаблону проектирования MVC? Что изменилось и  что осталось от нашего первоначального дизайна?

Насколько гибким является наш код? Легко ли он адаптируется? Сколько объектов нужно будет изменить, если мы вносем изменения в наш код? Например, что происходит, если мы хотим поддерживать запросы, предполагающие выбор из нескольких вариантов ответа? Что делать, если мы изменили файл хранилища данных?

Какие знания и навыки мы можем использовать и применить к нашему будущему коду?

<!-- [пример реализации mvc]: readme-assets/mvc-hospital-example.md -->
[шаблон дизайна Википедия]:http://en.wikipedia.org/wiki/Software_design_pattern
[wikipedia mvc]:https://ru.wikipedia.org/wiki/Model-View-Controller
