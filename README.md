# Money-can-not-buy-happiness
Money can not buy happiness
Проработав в Сбирбанке неделю, Маша стала совсем умирать от скуки. Чтобы хоть чем-то занять свободное от работы время (которого было слишком много), она установила на рабочий компьютер игру Sims: NSU Edition (в ней требуется создать персонажа-студента и следить за тем, чтобы он всегда был счастлив).

Когда в игре начались экзамены, очень много персонажей-студентов внезапно стали грустить. Маша, будучи филантропом, решила взломать игру, найти всех несчастных и осчастливить их. Покопавшись в коде, она выяснила, что счастье персонажа определяется восьмью признаками:

- Pass_exam (сдал экзамен)
- Ate_dumplings (бахнул пельменей)
- Slept_well (выспался)
- On_the_verge_of_expulsion (на грани отчисления)
- Writes_in_C (пишет код на Си)
- Writes_in_C_plus_plus (пишет код на С++)
- Watched_anime (смотрел аниме)
- Receives_a_scholarship (получает стипендию)

Для того, чтобы персонаж был счастлив, необходимо, чтобы он обладал хотя-бы одним зеленым признаком и не обладал сразу всеми красными признаками. Кроме того, если студент обладает синим признаком, то он счастлив в любом случае. Желтые признаки ни на что не влияют. Признаки каждого персонажа игры представлены числом типа char, и каждому признаку соответствует ровно один бит этого числа.

Пример
Персонаж, описанный числом 128 - счастлив: битовое представление числа - 10000000, что соответствует набору признаков {Pass_exam}. Поскольку у персонажа есть хотя-бы один зеленый признак и нет ни одного красного - он счастлив.

В то же время персонаж с признаками 240 - тоже счастлив. Битовое представление числа 240 - 11110000, что соответствует набору {Pass_exam**, Ate_dumplings**, Slept_well**, On_the_verge_of_expulsion**}. Поскольку есть зеленый признак, и при этом всего один красный признак из двух, человек счастлив.

Персонаж с признаками 25 - не счастлив. Битовое представление числа 25 - 00011001, что соответствует набору {On_the_verge_of_expulsion, Writes_in_C, Receives_a_scholarship}. Два красных признака из двух указывают на отсутствие счастья.

Формат ввода
​Первая строка содержит число N (N∈N,1≤N≤1e6) - количество персонажей в игре. Далее в каждой из N строк записано ровно одно число P i​, характеризующее i-го персонажа.

​

Формат вывода
​Программа должна содержать N символов: i-ый символ должен быть равен "1", если i-ый персонаж счастлив, и "0" в противном случае.
