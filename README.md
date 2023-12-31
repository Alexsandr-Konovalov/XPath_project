## Задача: Описать XPath'ы на первых двух страницах ("1. Выбор полиса" и "2. Оформление") для:

- Каждой кнопки;
- Каждого поля для ввода текста;
- Каждого чекбокса;
- Каждого датапикера;
- Логотипа "СБЕР СТРАХОВАНИЕ";
- Слайдера в блоке выбора суммы;
- Хедера "Что будет застраховано?";
- Текстовых блоков: "Мебель, техника и ваши вещи", "Падение летательных аппаратов и их частей";
- Каждой колонки в списка, который находится под хедером "Страховая защита включенная в программу".
> **P.S.: XPath'ы нужно писать для каждого элемента отдельно**

***

## Xpath для страницы «Выбор полиса»

| №  | Название                                                   | Xpath                                                                                                                           |
|----|------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
| 1  | Кнопка Квартира                                            | //*[@id="mat-button-toggle-1"]                                                                                                  |
| 2  | Кнопка Дом                                                 | //*[@id="mat-button-toggle-2"]                                                                                                  |
| 3  | Регион проживания                                          | //div[@class="mat-form-field-wrapper ng-tns-c61-0"] //*[@id="mat-input-0"]                                                      |
| 4  | Срок действия страхования (строка ввода)                   | //div[@class="mat-form-field-infix ng-tns-c61-1"]                                                                               |
| 5  | Срок действия страхования (кнопка открытия календаря)      | //*[@aria-label] //*[@aria-label="Open calendar"] //*[@mat-icon-button]                                                         |
| 6  | Сдается в аренду (да)                                      | //*[@id="mat-button-toggle-22"]                                                                                                 |
| 7  | Сдается в аренду (нет)                                     | //*[@id="mat-button-toggle-23"]                                                                                                 |
| 8  | Расположена на первом или последнем этаже (да)             | //*[@id="mat-button-toggle-25"]                                                                                                 |
| 9  | Расположена на первом или последнем этаже (нет)            | //*[@id="mat-button-toggle-26"]                                                                                                 |
| 10 | Установлена охранная  Сигнализация (да)                    | //*[@id="mat-button-toggle-28"]                                                                                                 |
| 11 | Установлена охранная Сигнализация (нет)                    | //*[@id="mat-button-toggle-29"]                                                                                                 |
| 12 | Слайдер в блоке выбора суммы                               | //*[@class="sbi-form__col-1"] //mat-slider                                                                                      |
| 13 | Поле ввода промокода                                       | //*[@id="mat-input-2"]                                                                                                          |
| 14 | Кнопка «Применить» В блоке «Промокод»                      | //*[@class="reg-button"]                                                                                                        |
| 15 | Кнопка «Оформить»                                          | //*[@class="form-actions"]  //*[@class="mat-focus-indicator mat-stroked-button mat-button-base mat-accent mat-button-disabled"] |
| 16 | Логотип "СБЕР СТРАХОВАНИЕ"                                 | //*[@class="sber-logo"]                                                                                                         |
| 17 | Хедер "Что будет застраховано?                             | //*[text()="Что будет застраховано?"]                                                                                           |
| 18 | Текстовый блок «Мебель, техника и ваши вещи»               | //*[text()=" Мебель, техника и ваши вещи "]                                                                                     |
| 19 | Текстовый блок «Падение летательных аппаратов и их частей» | //*[text()="Падение летательных аппаратов и их частей"]                                                                         |
| 20 | "Страховая защита включенная в программу" (Колонка №1)     | //div[text()="Чрезвычайная ситуация"]/ancestor::ul                                                                              |
| 21 | "Страховая защита включенная в программу" (Колонка №2)     | //div[text()="Стихийные бедствия"]/ancestor::ul                                                                                 |


***

## Xpath для страницы «Оформление»

| №  | Название                                      | Xpath                                                             |
|----|-----------------------------------------------|-------------------------------------------------------------------|
| 1  | Логотип "СБЕР СТРАХОВАНИЕ"                    | //div[@class="sber-logo"]                                         |
| 2  | Кнопка «Заполнить по Cбер ID»                 | //*[text()=" Заполнить по Сбер ID "]                              |
| 3  | Строка ввода фамилии                          | //*[@class="mat-form-field-wrapper ng-tns-c61-3"]                 |
| 4  | Строка ввода имени                            | //*[@class="mat-form-field-wrapper ng-tns-c61-4"]                 |
| 5  | Строка ввода отчества                         | //*[@class="mat-form-field-wrapper ng-tns-c61-5"]                 |
| 6  | Чекбокс «Отчество отсутствует»                | //*[@id="mat-checkbox-1-input"]                                   |
| 7  | Строка ввода даты рождения                    | //*[@id="mat-input-7"]                                            |
| 8  | Датапикер в строке ввода даты рождения        | //*[@class="mat-form-field-suffix ng-tns-c61-6 ng-star-inserted"] |
| 9  | Кнопка выбора пола (мужской)                  | //*[@id="mat-button-toggle-76-button"]                            |
| 10 | Кнопка выбора пола (женский)                  | //*[@id="mat-button-toggle-77"]                                   |
| 11 | Строка ввода серии паспорта                   | //*[@class="mat-form-field-flex ng-tns-c61-7"]                    |
| 12 | Строка ввода номера паспорта                  | //*[@class="contact-form__control number"]                        |
| 13 | Строка ввода даты выдачи паспорта             | //*[@class="mat-form-field-infix ng-tns-c61-9"]                   |
| 14 | Датапикер в строке ввода даты Выдачи паспорта | //*[@class="mat-form-field-suffix ng-tns-c61-9 ng-star-inserted"] |
| 15 | Строка ввода места выдачи паспорта            | //*[@class="contact-form__passport-item who-issued"]              |
| 16 | Строка ввода кода подразделения               | //*[@class="contact-form__passport-item department-code"]         |
| 17 | Строка ввода региона                          | //*[@class="contact-form__address-item region"]                   |
| 18 | Строка ввода города                           | //*[@class="contact-form__address-item city"]                     |
| 19 | Строка ввода улицы                            | //*[@class="contact-form__control street-input-field"]            |
| 20 | Чекбокс «Улица отсутствует»                   | //*[@id="mat-checkbox-2"]                                         |
| 21 | Строка ввода дом, литер, Корпус строение      | //*[@class="contact-form__control house"]                         |
| 22 | Строка ввода номера квартиры                  | //*[@class="contact-form__control apartment"]                     |
| 23 | Строка ввода номера телефона                  | //*[@class="mat-form-field-flex ng-tns-c61-17"]                   |
| 24 | Строка ввода электронной почты                | //*[@class="mat-form-field-wrapper ng-tns-c61-18"]                |
| 25 | Строка ввода   повтора электронной Почты      | //*[@class="contact-form__contact-item   info"]                   |
| 26 | Кнопка «Вернуться»                            | //*[text()="Вернуться"]                                           |
| 27 | Кнопка «Оформить»                             | //*[text()="Оформить"]                                            |

***

При помощи вкладки `Elements` отредактируйте какой-либо атрибут трех любых элементов на странице (шрифт, цвет, расположение, прочее — на усмотрение команды). Сделайте скрины этих элементов до и после редактирования, присвойте им названия: `1-before.png` — до, `1-after.png` — после.

- [1-after.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/1-after.png)
- [1-before.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/1-before.png)
- [2-after.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/2-after.png)
- [2-before.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/2-before.png)
- [3-after.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/3-after.png)
- [3-before.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/3-before.png)
- [4-after.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/4-after.png)
- [4-before.png](https://github.com/Alexsandr-Konovalov/XPath_project/blob/main/screens/4-before.png)

***
