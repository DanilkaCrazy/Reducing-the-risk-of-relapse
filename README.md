# Снижение рисков развития рецидива злокачественного новообразования
## Опубликованные авторские статьи на Хабре
[Профиль автора](https://habr.com/ru/users/FeLkan/)

[Как победить рецидив: путеводитель по полю битвы с онкологией](https://habr.com/ru/articles/866206/)

[Когда «тихая» ДНК громче гена: как избыточная ДНК регулирует экспрессию, ничего не делая](https://habr.com/ru/articles/863780/)

[Обзор недавно выпущенной модели Evo для анализа геномных данных](https://habr.com/ru/articles/865024/)

## Концепция и проектирование исследования:
База знаний (архив всех материалов исследования): https://disk.yandex.ru/d/7XdJ0gXXBTS2ow
### Цель: Выявить риски рецидива (повторное проявление) у послеоперационных пациентов.
### Описание исследования: 
После хирургического лечения злокачественных новообразований существует высокий риск рецидива (повторного проявления рака). Это может негативно сказаться на прогнозе и снижает выживаемость пациентов. Проект направлен на выявление факторов, влияющих на развитие рецидивов, и разработку стратегий их снижения, что в конечном итоге должно уменьшить количество случаев рецидива после оперативного лечения.

### Целевая аудитория:
1) Пациенты, перенесшие операции по удалению злокачественных новообразований. Эта группа нуждается в эффективных стратегиях для снижения риска повторного появления рака и улучшения прогноза.

2) Онкологи и хирурги. Врачи, занимающиеся лечением рака, смогут использовать результаты проекта для улучшения медицинской практики, персонализации лечения и мониторинга пациентов после операции.

3) Медицинские исследователи. Проект предоставляет данные и методы для анализа факторов, влияющих на риск рецидива, что может быть полезно для разработки новых терапий и клинических рекомендаций.

4) Медицинские учреждения и страховые компании. Понимание факторов риска рецидива может способствовать оптимизации планов лечения и снижения финансовой нагрузки на систему здравоохранения за счет предотвращения повторных заболеваний.

### Задачи: 
1) Поиск подходящих данных (TCGM, clinical data);
2) Анализ различных признаков (в том числе и генетических);
3) Формирование и проверка гипотез (стек: Python, RStudio, Bioconductor, Pandas и другие);
4) Документирование рабочих гипотез.

Datasets: https://disk.yandex.ru/d/FFfljjMKxa-K8g  
### Результат: Уменьшить количество рецидивов.

## Аналоги: способы снижения рецидива
Сравнение помогает оценить, какие методы более подходят для разных групп пациентов и на каких этапах лечения их применять.
### Способы:
- Адъювантная терапия: использование химиотерапии, радиотерапии или иммунотерапии после операции для уничтожения оставшихся раковых клеток.
- Генетическое тестирование: определение генетических мутаций, которые могут влиять на риск рецидива, и назначение целевой терапии.
- Мониторинг и раннее выявление: регулярные обследования и анализы для раннего выявления рецидива.
- Изменение образа жизни: отказ от курения, увеличение физической активности, здоровое питание.
- Психологическая поддержка: помощь пациентам в адаптации к послеоперационной жизни и снижении стресса.
- Персонализированная медицина: разработка индивидуальных планов лечения на основе генетических и клинических данных пациента.
  
### Таблица сравнения способов:
![Screenshot_2](https://github.com/user-attachments/assets/658b164f-6508-40d9-8cc3-de3f36262686)

Расширенный анализ конкурентов (с выводами и рекомендациями): https://disk.yandex.ru/i/8kfw2q6w81d9jg

### Описание критериев:
- Эффективность: насколько хорошо метод предотвращает рецидивы.
- Целевая группа: какие пациенты наиболее выигрывают от метода.
- Побочные эффекты: возможные нежелательные реакции или проблемы, связанные с применением метода.
- Время применения: когда и как долго используется метод.
- Стоимость: финансовые затраты на использование метода, как для пациента, так и для системы здравоохранения.

## Анализ данных
Целевой переменной в данном случае будет рецидив — повторное проявление заболевания после операции. Это может быть бинарная переменная (рецидив/нет рецидива) или временная переменная (время до рецидива).

![Screenshot_5](https://github.com/user-attachments/assets/38da2064-9ef9-4cc1-abb1-87b8cef7b2f8)

![Screenshot_1](https://github.com/user-attachments/assets/fc329aed-fc4d-4d95-a09e-b9b43bd327b6)


## Гены, влияющие на возникновение рецидива
- TP53 — один из наиболее известных генов-супрессоров опухолей. Мутации в TP53 часто ассоциируются с агрессивным течением опухоли и высоким риском рецидивов.
- BRCA1 и BRCA2 — мутации в этих генах увеличивают риск рецидива, особенно для пациентов с опухолями молочной и яичниковой желез.
- EGFR (эпидермальный фактор роста) — его мутации связаны с раком легких и некоторыми другими типами рака. Мутации могут влиять на прогноз и риск рецидива.
- KRAS — мутации в этом гене часто обнаруживаются при колоректальном и раке легких, что также может повлиять на риск повторного появления опухоли.
- PIK3CA — участвует в процессах клеточного роста и выживания. Мутации ассоциируются с более агрессивными опухолями, например, раком молочной железы.
- BRAF — мутации этого гена часто встречаются при меланоме и колоректальном раке и могут способствовать устойчивости опухоли к лечению, что увеличивает риск рецидива.

## Анализ зависимости рецидива от числа мутаций

![Screenshot_1](https://github.com/user-attachments/assets/c187898b-69d5-49d5-9775-cb7d78d722d0)

На графике показано распределение количества мутаций в зависимости от статуса выживаемости пациентов. Видно, что пациенты с более высоким количеством мутаций могут чаще оказываться в группе с повышенным риском (умершие пациенты). Это может указывать на то, что большое количество мутаций ассоциируется с худшим прогнозом и потенциально более высоким риском рецидива.

## Как собирались данные?
Первое, что нужно сделать - это перейти на сайт [TCGA (The Cancer Genome Atlas)](https://www.cancer.gov/ccg/research/genome-sequencing/tcga):

![Screenshot_10](https://github.com/user-attachments/assets/3930a2c7-dee0-41ec-bdb3-71e0185e2808)

Атлас ракового генома (англ. The Cancer Genome Atlas, TCGA) или АРГ — проект, целью которого является систематизация данных о генетических мутациях, приводящих к возникновению рака. Систематизация проводится с помощью секвенирования и методов биоинформатики. Данный проект — совместная работа Национального Института Рака и Института Исследований Генома Человека, США. Подробнее можно почитать в [Википедии](https://ru.wikipedia.org/wiki/%D0%90%D1%82%D0%BB%D0%B0%D1%81_%D1%80%D0%B0%D0%BA%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE_%D0%B3%D0%B5%D0%BD%D0%BE%D0%BC%D0%B0).

После перехода на сайт, обратим внимание на встречающий нас экран. Нужно немного спуститься ниже. Нажать на кнопку ["Access Data"](https://portal.gdc.cancer.gov/).

![Screenshot_11](https://github.com/user-attachments/assets/35dc8fcb-382d-4249-9440-d4cfb776971f)

Сверху слева переходим в ["Аналитический центр"](https://portal.gdc.cancer.gov/analysis_page?app=):

![Screenshot_12](https://github.com/user-attachments/assets/64d33a2f-3d69-4cde-a564-ecdcffca558f)

К странице, которую мы видим сейчас, еще обязательно вернемся! Нам нужно создать когорту, другими словами, собрать интересующие нас данные. Ведь всего кейсов на данный момент (10.10.2024) насчитывается около 44736, это случаи заболевания рака, которые были тщательно изучены, по этим кейсам и собирались данные. Абсолютно все данные могут стать для нас избыточны, поэтому выбираем интересующие нас через когорту:

![Screenshot_13](https://github.com/user-attachments/assets/0fda9bd9-fd9e-4403-a817-2a41b5069adf)

И вот мы нажали на ["Cohort Builder"](https://portal.gdc.cancer.gov/analysis_page?app=CohortBuilder&tab=general) и видим следующие общие данные:

![Screenshot_15](https://github.com/user-attachments/assets/8627cc82-367b-4e4d-bf3b-87d5347b241c)

Если вы понимаете английский на среднем уровне, проблем возникать с переводом не должно. В случае, если вы используете Google - пользуйтесь встроенным переводчиком. Итак, о чем это я? Да. Точно. Переходим в ["Avalaible Data"](https://portal.gdc.cancer.gov/analysis_page?app=CohortBuilder&tab=available_data). Меня интересуют следующие методы, например, RNA-seq (RNA Sequencing) — секвенирование РНК и WGS (Whole Genome Sequencing) — полногеномное секвенирование. Я их выбрал (для просмотра всех данных потребуется нажать "more" - далее):

![Screenshot_16](https://github.com/user-attachments/assets/03e414fd-c97b-4a79-9791-597e1bf81117)

Теперь возвращаемся назад в ["Аналитический центр"](https://portal.gdc.cancer.gov/analysis_page?app=):

![Screenshot_17](https://github.com/user-attachments/assets/f7bc2444-b435-470e-b14f-8f4bc93d2429)

Итак, становится очевидным, что количество кейсов поменялось - их стало меньше, из-за того что мы сократили выборку. Изначально нам доступны абсолютно все кейсы по всем данным. Это сделано для того, чтобы постоянно не приходилось нажимать абсолютно на все галочки (поверьте, это очень трудно).

Переходим к визуализациям - самый важный и интересный этап. Почему важный? Помогает докопаться до сути и быстро понять представленные данные. 

![Screenshot_18](https://github.com/user-attachments/assets/7bf66c68-609d-425e-9684-2c1e46ffc446)

И вот, графики уже перед нами. Можно спуститься чуть ниже и посмотреть информацию по генам.

![Screenshot_19](https://github.com/user-attachments/assets/002d9f27-1def-4067-9d87-e6d63fb89d08)

Предлагаю заглянуть еще и кластеризацию экспрессии генов:

![Screenshot_20](https://github.com/user-attachments/assets/20bcf4b7-4914-4a1e-b860-52aee3e2e356)

Тут нас ожидает тепловая матрица корреляции. Но данных в ней ужасно много и лучше сократить их объем:

![Screenshot_6](https://github.com/user-attachments/assets/9139cc79-f1b3-47ea-9e91-305f1b0d9d05)

Далее, выбираем "скачать" - формат TSV:

![Screenshot_21](https://github.com/user-attachments/assets/f86be88b-d4a0-440f-8624-4fb5222259b1)

И вот уже успешно скачался файл с названием: HierClaster.2024-12-09.tsv. Для удобства анализа данных переведем его в csv формат. Теперь запомним, в этом файле показаны гены и их корреляция (вещественное число). Есть необходимость в будущем объединить их с другими данными с сайта TCGA. В моем случае, это были аликвоты.

## Интерпретация данных: что такое аликвоты?
Аликвоты — это небольшие, точно измеренные порции или образцы биологического материала, которые отбираются из исходного объема для анализа, экспериментов или хранения. В контексте биомедицинских исследований и онкологии, таких как проекты TCGA (The Cancer Genome Atlas), аликвоты часто представляют собой:
* Образцы тканей
* Образцы жидкостей
* ДНК или РНК
* Клеточные линии или другие культуры

В проектах вроде TCGA аликвоты служат основой для анализа геномных, транскриптомных и эпигенетических данных. Каждая аликвота связана с конкретным пациентом и его клиническими характеристиками, что делает их ключевыми элементами для интеграции молекулярных и клинических данных.

Зачем используют аликвоты:
- Сохранение ресурсов: Вместо работы с большим объемом материала, исследователи используют небольшие порции.
- Стандартизация: Аликвоты позволяют унифицировать анализы и снизить вариабельность.
- Многократное использование: Несколько аликвот одного образца могут быть использованы для разных экспериментов.
- Долговременное хранение: Аликвоты часто замораживают или хранят в специальных условиях для будущих исследований.

## Планирование работ
В течение семестра задачи по работам в проекте были распределены в зависимости от занимаемых ролей участниками:

![Screenshot_28](https://github.com/user-attachments/assets/89cdb97a-ffba-4120-a53c-4d8dd01921cf)

## Выявленные гены

![Screenshot_2](https://github.com/user-attachments/assets/46bb657a-2334-4b8f-bdb9-c823471d62e0)













