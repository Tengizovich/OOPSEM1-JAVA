Урок 1. Принципы ООП: Инкапсуляция, наследование, полиморфизм
Задание: Реализовать, с учетом ооп подхода, приложение
Для проведения исследований с генеалогическим древом. Идея: описать некоторое количество компонент, например: модель человека компонента хранения связей и отношений между людьми: родитель, ребёнок - классика, но можно подумать и про отношение, брат, свекровь, сестра и т. д. компонент для проведения исследований дополнительные компоненты, например отвечающие за вывод данных в консоль, загрузку и сохранения в файл, получение\построение отдельных моделей человека Под “проведением исследования” можно понимать получение всех детей выбранного человека.

Решение
В классе "Person" создали модель человека, который имеет имя и фамилию. В enum "Relation" указываем возможные родственные связи - родитель, брат, сестра и т.д.

Класс "Relationship" создает непосредственно сами родственные связи двух людей - кем первый человек приходится второму и наоборот. Данные связи хранятся в классе "FamilyTree".

В "Main" создал 8 условных человек с их родственными связями. Используя класс "Search" выводим на печать родственные связи для "Человека8".