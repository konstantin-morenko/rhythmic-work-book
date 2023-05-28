
# Шаблон для проектов на основе just-the-docs-reborn

## Уровни вложенности

Для организации используются папки и файлы.  Цифра в скобках означает уровень вложенности.

- index.md (1)
- chapter/
  - index.md (1)
  - theme.md (2)
  - theme/
    - index.md (2)
    - subtheme.md (3)
    
### Front Matter

Порядок следования правил:
- title
- grand_parent
- parent
- nav_order
- has_children
- остальные

Уровень 1

    title: Шаблон
    nav_order: 1
    has_children: true
    
Уровень 2

    title: Тема
    parent: Шаблон
    nav_order: 1
    has_children: true
    
Уровень 3

    title: Подтема
    grand_parent: Шаблон
    parent: Тема
    nav_order: 1

