Aplikacja jak każdą w Java uruchamiamy z poziomu klasy zawierającej metodę _Main()_, w tym przypadku _ApkaKubaApplication_, w klasie tej zawarta jest także adnotacja 
_@SpringBootApplication_ inicjująca Spring Framework.

Kontrolę nad tym co wyświetla nasza aplikacja pełni klasa _HelloController_, z odpowiednią adnotacją _@Controller_ informującą o tym Springa. Aplikacja obsługuje wejście na adresy
localhost:8080/ oraz localhost:8080/greeting i w zależności od adresu wyświetla inne rzeczy. W pierwszym przypadku jest to tylko komunikat 
"Hello Vistula, in my first Spring controller.".

W drugim jest to strona _greeting.html_ wraz z obrazkiem _vistula.png_ obydwa te elementy znajdują się w katalogu _resources_ czyli zasobach naszej aplikacji.
Z poziomu klasy _HelloController_po wejściu użytkownika w odpowiedni adres metoda _greeting()_ zwraca odpowiedni plik HTML który jest wyświetlany w przeglądarce.