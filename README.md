# System do zarządzania firmą wypożyczającą pojazdy
1. Opis tematu aplikacji
   
    Aplikacja służy do zarządzania flotą pojazdów w wypożyczalni. System obsługuje różne typy pojazdów, wylicza kosztów dziennego wypożyczenia, zarządza bazą klientów oraz realizuje rezerwacje

2. Lista klas i ich odpowiedzialności
   
   -Pojazd – klasa bazowa zawierająca wspólne cechy dla wszystkich środków transportu
   
   -SamochodOsobowy – klasa szczegółowa dziedzicząca po `Pojazd`, rozszerzona o pojemność bagażnika
   
   -Motocykl – klasa dziedzicząca po klasie `Pojazd`, zawierająca informację o typie napędu
   
   -Klient – klasa reprezentująca użytkownika systemu z unikalnym numerem ID i jego danymi
   
   -Wypozyczenie – klasa reprezentująca operację wynajmu

4. Opis relacji między klasami
   
    -Agregacja - Klasa `MenedzerFloty` przechowuje listy obiektów typu `Pojazd` oraz `Wypozyczenie`. Pojazdy i rezerwacje mogą istnieć niezależnie, ale manager nimi zarządza
  
    -Kompozycja - : Klasa `Wypozyczenie` posiada referencje do obiektów `Klient` oraz `Pojazd`. Wynajem nie może istnieć bez przypisanego klienta i auta
  
    -Przekazywanie obiektu jako parametr - Metoda `ZarejestrujWypozyczenie` przyjmuje jako parametry obiekty klas `Klient` oraz `Pojazd`, aby powiązać je w nowym obiekcie rezerwacji

4. 


    Michał Spicer 72373 Jaworzno
