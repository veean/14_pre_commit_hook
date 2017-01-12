# Quadratic Equations Solver

Перехватчик pre-commit hook используется для того чтобы убедиться, что вы запустили тесты, или 
проверить в коде ещё что-нибудь.
Данный pre-commit стартует при попытке коммита, запускает файл tests.py и 
при наличии ошибок прерывает коммит с уведомлением о фейле.

# To-Read

Подробнее про перехватчики : 
* [Git - Перехватчики в Git](https://git-scm.com/book/ru/v1/%D0%9D%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-Git-%D0%9F%D0%B5%D1%80%D0%B5%D1%85%D0%B2%D0%B0%D1%82%D1%87%D0%B8%D0%BA%D0%B8-%D0%B2-Git)
* [Git Hooks | Atlassian Git Tutorial](https://ru.atlassian.com/git/tutorials/git-hooks/)

# Использование скрипта

* Переходим в папку c проектом, перемещаем скрипт pre-commit в папку .git/hooks/ , 
 даем права на выполнение:
    
    
    `~ cd 14_pre_commit_hook
    
    ~ mv pre-commit .git/hooks/
    
    ~ chmod +x pre_commit`

* При вызове `git commit` или `git commit -m` хук стартует и запускает tests.py.
  Если все ОК - коммит выполняется. Если тесты упали - коммит прервется с предупреждением.


# Зависимости 
Версия python 3.5 и выше.

# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)
