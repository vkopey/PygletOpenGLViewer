# PygletOpenGLViewer
Simple 3D OpenGL object viewer based on pyglet https://bitbucket.org/pyglet/pyglet.

Простий переглядач 3D об'єктів OpenGL на основі pyglet.

Бібліотека pyglet (версія 1.3.1) може бути установлена за допомогою менеджера пакетів pip:

pip install pyglet

Метою проекту є демонстрація можливості pyglet для швидкої розробки інтерактивних мультимедійних програм з графікою OpenGL на прикладі простої програми. Програма може бути використана як шаблон для створення складніших програми.

Спочатку імпортуються необхідні модулі і функції бібліотеки pyglet. Клас MyWindow успадковує клас Window і описує вікно програми. Функція-конструктор __init__ викликається під час створення екземпляра вікна. Функція on_resize викликається під час зміни розміру вікна. В ній установлюється порт виведення і режим перспективної проекції. Функція on_draw викликається під час необхідності перерисування об’єктів і рисує повернутий навколо осей X, Y графічний об’єкт (трикутник) шляхом виклику функції drawObject. Функція on_mouse_drag викликається під час перетягування вказівника миші з натиснутою лівою кнопкою. В ній змінюються кути повороту навколо осей X, Y на величини переміщень вказівника миші dx, dy.
