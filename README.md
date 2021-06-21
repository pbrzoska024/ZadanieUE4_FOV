# ZadanieUE4_FOV
Repozytorium przeznaczone na zadanie z unreal engine
[wersja projektu : 4.26.2]
[czas : 16.06 - 21.06]


WorkFlow na czas obecny:

* [1.Wykonano linetracing punktów]
* [2.Utworzono na  podstawie ich wyników procedural mesha]
* [3.Utworzono kontroler i postac AI]
* [4.Dostosowano utworzone FOV z komponentem widzenia i jego zasięgiem]
* 
* [5.Napisano serwis, taski i dekoratory dla AI]
* [6.Utworzono punkty które ai będzie patrolować]
* [7.Utworzono warunki których Ai będzie decydowac kiedy zobaczy gracza]
* [8.Utworzono strefe cienia dzięki któremu gracz może się chować]
* 



Poniżej przestawiono diagram architektury projektu
![ZadanieAiDiagram (2)](https://user-images.githubusercontent.com/53401206/122745061-e720be00-d288-11eb-940c-864ce8b38cef.png)


Screen przestawiający patrolujące AI
![image](https://user-images.githubusercontent.com/53401206/122743664-7927c700-d287-11eb-8bcc-1fc52e3340ca.png)
![image](https://user-images.githubusercontent.com/53401206/122744690-885b4480-d288-11eb-8f8c-0d9de3770063.png)

Drzewo zachowań:
![image](https://user-images.githubusercontent.com/53401206/122745465-53032680-d289-11eb-896c-9673d7d64261.png)

Ai patroluje wybrane punkty (ATargetPoints).
Jeżeli gracz jest w odległości do 5m, Ai od razu przystępuje do chase
Jeżli gracz jest w odległości od 10m do 15m, Ai czeka chwilę i następnie przystepuje do chase
Jeżeli Ai zgubiło gracza lub gracz wszedł w cień, Ai idzie w ostatnie znane miejsce gdzie widziało gracza, a następnie wraca do patrolowania.


