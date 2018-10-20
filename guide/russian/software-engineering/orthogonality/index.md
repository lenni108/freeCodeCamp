---
title: Orthogonality
localeTitle: Ортогональность
---
## Ортогональность

В программной инженерии система считается ортогональной, если изменение одного из ее компонентов изменяет только состояние этого компонента. Например, рассмотрим программу с тремя переменными: a, b и c. Изменение значения a не должно изменять значение b или c, если они независимы. Это свойство особенно важно при отладке программы, поскольку вы полагаетесь на сужение числа движущихся частей программы, чтобы определить основную причину проблемы.

См. Следующую цитату из «Искусство программирования UNIX» Эрика С. Раймонда,

> Ортогональность - одно из самых важных свойств, которое может помочь сделать даже сложные конструкции компактными. В чисто ортогональном дизайне операции не имеют побочных эффектов; каждое действие (будь то вызов API, вызов макроса или языковая операция) меняет только одну вещь, не затрагивая других. Существует один и только один способ изменить каждое свойство любой системы, которую вы контролируете.

Ортогональность - это принцип разработки программного обеспечения для написания компонентов таким образом, что изменение одного компонента не влияет на другие компоненты. Это сочетание двух других принципов, а именно: сильное сцепление и свободная связь.

Ортогональность - это термин, заимствованный из математики. Например, две линии ортогональны, если они перпендикулярны. При разработке программного обеспечения две компоненты ортогональны, если изменение одного не влияет на другое.

Применение этого понятия к классам или другим разделам кода приводит к уменьшению сцепления. Чтобы быть ортогональным, два класса не могут зависеть от реализации друг друга. Они также не могут передавать глобальные данные. Изменение внутренних элементов одного класса не влияет на другой класс. Компоненты должны быть независимыми и иметь только одну ответственность.

Рассмотрим метод, который читает список чисел из файла и возвращает их в отсортированном порядке. Теперь требования изменяются, а числа находятся в базе данных. Изменение этого метода для доступа к базе данных приведет к изменению кода клиента. Если бы это были два разных метода, то новый источник не повлиял бы на метод сортировки. Только код клиента должен знать источник чисел.

### Сильная сплоченность

Внутри программного компонента код должен быть сильно связан. Это указывает на правильность разделения кода. Если у компонента есть две или более относительно разъединенные части, это может указывать на то, что эти части должны быть в другом компоненте или сами по себе.

### Слабая связь

Между программными компонентами должно быть несколько соединений. Если два компонента сильно связаны, это может указывать на то, что они должны быть одним компонентом или что их нужно разделить на несколько компонентов.

#### Дополнительная информация:

*   [Ортогональность (программирование) | Википедия](https://en.wikipedia.org/wiki/Orthogonality_(programming))
*   [Принципы ортогонального объектно-ориентированного программирования | jasoncoffin.com](http://www.jasoncoffin.com/cohesion-and-coupling-principles-of-orthogonal-object-oriented-programming/)
*   [GRASP - объектно-ориентированные принципы проектирования | Википедия](https://en.wikipedia.org/wiki/GRASP_(object-oriented_design)

Переполнение стека: что такое ортогональность ?. https://stackoverflow.com/questions/1527393/what-is-orthogonality