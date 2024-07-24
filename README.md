Для улучшения качества кода:
* Вынес параметры поиска в отдельную переменную search_params для прямого обращения
* Убрал не нужные проверки на None или '' так как они усложняют чтения но при этом возвращают False
* Оптимизировал запросы используя values_list для получения списка id
* Использовал exist() для проверки на наличие элемента
* Использовал линтер для повышения читаемости (Я бы встроил его в CI/CD пайплайн)

Разработчику я бы сказал что стоит:
* Немного поработать над неймингом
* Выделять отдельно то что используется множество раз (DRY)
* Прочитать какой результат дает проверка объектов в if выражении для упрощения кода