# Портфолио: аналитик данных

## Обо мне 

Привет! Меня зовут Елена, я начинающий аналитик данных. 
В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.
<br>

## Навыки и технологии
- Инструменты анализа данных: ``SQL``, ``Excel``  
- Системы управления базами данных: ``MySQL``, ``PostgreSQL``



## Проекты
<p> Проект 1: Калькулятор юнит-экономики онлайн-школы</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1: Настроить в калькуляторе учет корректировок планов маркетинга</li>
  <li>Задача №2: Пересчитать план найма преподавателей</li>
</ol>

<p>Как решала: 
<ol>
  <li>Задача №1: добавила в список параметров калькулятора показатель "Поправочный коэф-т на привлечение"; установила значение этого показателя по умолчанию как 100% и добавила возможность изменять этот показатель для расчётного периода 05.21-04.22; настроила динамический расчёт количества новых студентов за период 05.21-04.22 с поправкой на этот коэффициент; если для 05.21-04.22 он равен 120%, то в каждый месяц этого периода рассчётное значение количества новых студентов должно быть больше на 20%; просчитала сценарий, при котором планы маркетинга будут увеличены на 12% (настройки остальных показателей не меняются)<p>
 <li>Задача №2: добавила в калькулятор Найма преподавателей возможность изменять входные параметры: Пропускную способность П и Retention П - с помощью дополнительного столбца с процентными изменениями, как это сделано на Главном листе с основным калькулятором Юнит-экономики; сделала поправку в расчёте общей пропускной способности - изменила формулу так, чтобы отразить, что новые преподаватели в первый месяц своей работы могут проводить только половину уроков от средней пропускной способности преподавателя, задаваемой параметром; обновила прогнозное количество уроков, добавив новые значения из Задачи 1 (полученные после поправки на планы маркетинга); просчитала сценарий, при котором Пропускная способность П увеличится на 15 процентов, а Retention П упадёт на 2 процента; с помощью Поиска решений составила новый план найма с ограничением: за месяц нельзя нанять более 70 преподавателей
</ol>

> <a href="https://github.com/Skyproportfolio/data-analytics-5month/blob/main/Проект%20№1.xlsx">Ссылка на проект</a>

<p>Выводы (итоги):<p>
<ol>
  <li>Итог №1: Обновленный лист с калькулятором + новое расчётное количество студентов на 04.2022</li>
  <li>Итог №2: Обновлённый план по найму - с количеством новых преподавателей по месяцам за период с 05.2021 по 04.2022</li>
</ol>
<br> 

<p> Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача: Ответить на вопрос: насколько используемая бизнес-модель эффективна с точки зрения финансовой составляющей? </li>
</ol>

<p>Как решала: посчитала юнит-экономику продукта и предложила сценарий по настройке параметров для выхода на 25-процентную маржинальность, собрала наглядную визуализацию, где показано, кто, где и в каком объеме смотрит фильмы на платформе<p>

> <a href="https://drive.google.com/drive/folders/11HcEeqniyrCMjuwHZ0GLysX0A2SEv-_x">Ссылка на проект</a>
 
<p>Выводы (итоги):<p>
<ol>
  <li>Итог: Кинотеатр работает в минус. На данном этапе развития каждая подписка дает нам -94% прибыли. Предложен сценарий по настройке параметров юнит-экономики продукта для выхода на 25%-ную маржинальность: увеличен Retention на 12%, увеличена фактическая цена подписки на 10 % за счет сокращения объема скидок, уменьшены средний САС на 39% и Fixed Costs на 1 подписку на 10%</li>
</ol>
<br> 

<p> Проект 3: Когортный анализ онлайн-кинотеатра с помощью SQL</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1: Построить гистограмму с распределением количества покупок по полям is_trial и name_partner, добавить к графику срез, на котором можно выбрать, на каких по счету покупках в рамках клиента построена гистограмма (только на первых; только на вторых; на всех, кроме первых, и т. д.)</li>
  <li>Задача №2: Дополнить код таким образом, чтобы получились винтажные доходимости, и визуализировать полученные результаты в Excel</li>
</ol>

<p>Как решала(-а): 
<ol>
  <li>Задача №1: с помощью функции row_number проставила ранги покупок в рамках каждого клиента по времени; сгруппировала полученные результаты: нашла количество строк для каждого значения полей is_trial, name_partner и ранг (group by по трем полям одновременно); перенесла полученные результаты в Excel, визуализировала их и поле «ранг» сделала срезом
  <li>Задача №2: для каждого партнера рассчитала, какой процент клиентов дошел до второй покупки, до третьей покупки и т. д., используя конструкцию sum(case when…); нарисовала график, на котором каждая линия показывает своего партнера<p>
</ol>

> <a href="https://drive.google.com/drive/folders/1wdD-mfSeIsHWgrMLJz8Tv_ClAuP_EAOQ?usp=sharing">Ссылка на проект</a>

  <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1: Построенная гистограмма с распределением количества покупок со срезом, на котором можно выбрать ранг покупки</li>
  <li>Итог №2: Визуализация винтажных доходимостей клиентов</li>
</ol>

<br> 
<p>Проект 4: Построение витрины для модели машинного обучения в банке </p> 
<p>Что нужно было сделать: задача №1.<p>
  
<p>Как решала(-а): краткое описание решения (автореферат)<p>

> <a href="https://drive.google.com/drive/folders/1QOk5AAh6x7jK_yHgfKI2sUFYR7AWUi5u">Ссылка на проект</a>
(ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)
  
 <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1</li>
  <li>Итог №2</li>
</ol>
<br> 


<p>Проект 5: Моделирование изменения балансов студентов</p> 
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1</li>
  <li>Задача №2.</li>
</ol>

<p>Как решала(-а): краткое описание решения (автореферат)<p>

> <a href="https://github.com/Skyproportfolio/data-analytics-5month/blob/main/Проект%205.xlsx">Ссылка на проект</a>
(ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)
 
 <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1</li>
  <li>Итог №2</li>
</ol>

## Контактная информация
- Email: perminova.elenanik@yandex.ru
