# System do zarządzania firmą wypożyczającą pojazdy
1. Opis tematu aplikacji
Aplikacja służy do zarządzania flotą pojazdów w wypożyczalni. System obsługuje różne typy pojazdów, wylicza kosztów dziennego wypożyczenia, zarządza bazą klientów oraz realizuje rezerwacje

2. Lista klas i ich odpowiedzialności
*Pojazd – klasa bazowa zawierająca wspólne cechy dla wszystkich środków transportu
*SamochodOsobowy – klasa szczegółowa dziedzicząca po `Pojazd`, rozszerzona o pojemność bagażnika
*Motocykl – klasa dziedzicząca po klasie `Pojazd`, zawierająca informację o typie napędu
*Klient – klasa reprezentująca użytkownika systemu z unikalnym numerem ID i jego danymi
*Wypozyczenie – klasa reprezentująca operację wynajmu

Michał Spicer 72373 Jaworzno
