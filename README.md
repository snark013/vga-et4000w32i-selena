# Selena
Tseng 4000 W32i based ISA VGA card.
Not tested.



## Specification -
- Быстрая работа с памятью в MS-DOS
- Полностью VGA совместима
- MS Windows Acceleration
- True Color RAMDAC
- Два варианта конфигурации памяти 
    - 1 Mb non-interleave mode (наиболее беспроблемная конфигурация) - устанавливаются две микросхемы памяти U4 и U5.
    - 2 Mb interleave mode (наиболее быстрая конфигурация, стабильность может зависить от используемой памяти) - устанавливаются все четыре 
    микросхемы памяти U1, U2, U4 и U5.
- 16-bit ISA двухслойная плата


## Changes
- Version 0.9.2
    - оптимизация расположения элементов 

    память разнесена на две стороны, более оптимальные шины к памяти, изменено подключение к памяти, 
    память теперь подключена не так как у Александра Грозы, возможен вариант конфигурации с двумя чипами памяти на 1Mb - такой вариант
    позволяет использовать практически любую память даже ту которая не работает в режиме interleave 2Mb как у Groza.
    - все конденсаторы меньше чем 0.1u заменены на 0805,
    - изменена нумерация элементов.
- Version 0.7
    - возможно для RAMDAC запаять панельку PLCC44,
    - добавлен альтернативный футпринт вариант для video clock generator.

    U3 можно заменить на U'3 (CH9294E бывает как DIP так и SOIC, так же можно применить ICS2494-304 в SOIC)
- Version 0.3
    - первая версия.


## Related projects
Данный проект основан на проекте Alexandru Groza EXCELGRAPH ISA VIDEO DISPLAY CONTROLLER -

https://www.alexandrugroza.ro/microelectronics/system-design/isa-video-display-controller/index.html
