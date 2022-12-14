changes.md
# ЗАЯВКА
### Функциональные требования:
  + Создание тестов для закрепления изученного
### Создание иероглифа:
  * Было:  
    + добавления данных об иероглифе (изображение иероглифа, изображение значения, звучание, транскрипция, перевод, словосочетание, перевод словосочетания)
  * Стало: 
    + добавления данных об иероглифе (иероглиф, транскрипция, перевод, словосочетание, перевод словосочетания, картинка, аудио)
### Содержание урока:
  * Было:  
    + Проверка знаний
    + Материал урока представляет собой 3D модель куба, анимированную с помощью WebGL, на 6 сторонах которого: иероглиф, транскрипция (с кнопкой озвучивания), перевод, картинка, словосочетание на русском, перевод словосочетания на китайский (с кнопкой озвучивания).
  * Стало: 
    + Выбор теста для закрепления материала урока
    + Проходение тестов для проверки своих знаний
    + Материал урока представляет собой 3D модель куба, анимированную с помощью WebGL, на 5 сторонах которого: иероглиф (с кнопкой озвучивания), картинка и транскрипция (с кнопкой озвучивания), перевод (с кнопкой озвучивания), словосочетание на русском, перевод словосочетания на китайский (с кнопкой озвучивания).
### Тренажеры:
  * Было: 
    + выбор картинки по иероглифу
    + выбор иероглифа по картинке
    + 6 вариантов тренажера с кубиком, на котором пропущена одна из сторон, которую должен выбрать обучающийся из предложенных вариантов.
    + Проверка знаний будет основана на тренажерах (с кубиком). При прохождении сообщается, сколько слов выучил пользователь, что также отображается в статистике по курсу и в статистике учителя.
  * Стало: 
    + выбор варианта иероглифа по аудио
    + выбор варианта словосочетания на китацском по аудио
    + 12 вариантов тренажера с кубиком, на котором пропущена одна из сторон, которую должен выбрать обучающийся из предложенных вариантов.
    + Проверка знаний будет основана на тренажерах. При прохождении сообщается, сколько слов выучил пользователь, что также отображается в статистике по курсу и в статистике учителя.
    + Новые тренажеры:  
     - выбор варианта иероглифа по картинке
     - выбор варианта картинки по иероглифу
     - выбор варианта иероглифа по транскрипции
     - выбор варианта транскрипции по иероглифу
     - выбор варианта транскрипции по картинке
     - выбор варианта картинки по транскрипции

# ПОЛЬЗОВАТЕЛЬСКИЕ СЦЕНАРИИ
### [ Сценарий 2 - Работа со словарем ]
  * Было:
    + 2 Учитель может поставить галочку "отображать только мои слова"
    + 3 Учитель может найти слово по иероглифу или переводу
    + 4 Учитель может отсортировать слова по дате добавления
    + 5 Учитель может отсортировать слова в алфавитном порядке относительно иероглифа или перевода
  * Стало: 
    + 2 Учитель может нажать на кнопку "показать только мои слова"/"показать только чужие слова"/"показать все слова"
    + 3 Пользователь может найти слово по иероглифу или переводу
    + 4 Пользователь может отсортировать слова по дате добавления
    + 5 Пользователь может отсортировать слова в алфавитном порядке относительно иероглифа или перевода

### [ Сценарий 3 - Добавление слов в словарь ]
  * Было:
    + 4 Учитель добавляет картинки на стороны кубика
    + 5 Опционально учитель добавляет аудио файлы на стороны кубика
    + 6 Если учитель заполнил не все поля, система не позволяет сохранить слово
    + 7 Если в словаре уже существует слово с такими же иероглифом и переводом, система предупреждает учителя (но учитель все равно может сохранить слово)
  * Стало: 
    + 4 Учитель вводит транскрипцию слова
    + 5 Учитель вводит словосочетание на китайском
    + 6 Учитель вводит словосочетание на русском
    + 7 Учитель добавляет картинку для слова
    + 8 Опционально учитель добавляет аудио файлы для транскрипции/перевода/словосочатания слова
    + 9 Если учитель заполнил не все поля, система не позволяет сохранить слово
    + 10 Если в словаре уже существует слово с такими же иероглифом и переводом, система предупреждает учителя (но учитель все равно может сохранить слово)

### [ Сценарий 4 - Создание курса ]
  * Было:
    + 6 Если курс создан, Учитель может изменять, добавлять и удалять уроки.
    + 7 Если курс создан, Учитель может посмотреть статистику учеников
  * Стало: 
    + 6 Если курс создан, Учитель может изменять, добавлять и удалять уроки - запускается Сценарий 5
    + 7 Если курс создан, Учитель может добавить учеников к курсу, нажав на кнопку - запускается Сценарий 7
    + 8 Если курс создан, Учитель может посмотреть статистику учеников

### [ Сценарий 5 - Создание урока ]
  * Было:
    + 9 Учитель должен выбрать какие виды тренажеров будут созданы для этого урока
  * Стало: 
    + 9 Учитель может выбрать виды тренажеров, котрорые будут добавлены этому уроку
  * Новое:
    + 10 Учитель может выбрать виды тестов для проверки знаний, котрорые будут добавлены этому уроку
    + 13 Если урок создан, учитель может добавлять и удалять тесты.

### [ Сценарий 7 - Добавление учеников к курсу ]
  * Было:
    + 7 Если учитель хочет удалить ученика из курса, он должен нажать на кнопку удаления пользователя рядом с нужным учеником.
  * Стало: 
    + 7 Если учитель хочет удалить ученика из курса, он должен нажать на имя уже добавленного ученика еще раз.

### [ Сценарий 10 - Просмотр материалов урока учеником ]
  * Было:
    + 4 Если ученик не отключил функцию обучения, после просмотра одной стороны, рядом с кубом появляются стрелки, указывающие на возможность поворота
  * Стало: 
    + 3 Если ученику непонятно, как управлять кубиком, он может нажать на кнопку с вопросом, которая покажет инструкцию

### [ Сценарий 11 - Просмотр тренажеров и проверка знаний учеником ]
* Было:
    + [ Сценарий 11 - Просмотр материалов и проверка знаний учеником ]
    + Ученик должен нажать на кнопку "Проверка знаний" в урока
* Стало: 
    + [ Сценарий 11 - Просмотр тренажеров и проверка знаний учеником ]
    + Ученик должен выбрать тест из урока

