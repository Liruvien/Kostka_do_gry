# Kostka_do_gry

## Opis projektu

**Kostka do gry** to program symulujący rzuty różnymi rodzajami kostek, co jest często używane w grach planszowych i RPG. Program obsługuje zapis rzutów kostką w skróconym formacie, na przykład `2D10+20`, co oznacza dwa rzuty dziesięciościenną kostką (D10) z dodaniem modyfikatora 20 do wyniku końcowego.

## Składnia kodu

Format zapisu dla rzutów kostką:
xDy+z

Gdzie:
- `y` – typ kostki (np. D6, D10, D20),
- `x` – liczba rzutów (jeśli rzucamy raz, ten parametr jest pomijalny),
- `z` – modyfikator dodawany lub odejmowany od wyniku rzutów (opcjonalnie).

### Przykłady zapisu:
- `2D10+10`: wykonaj dwa rzuty dziesięciościenną kostką i dodaj 10 do wyniku,
- `D6`: wykonaj pojedynczy rzut sześcienną kostką D6,
- `2D3`: wykonaj dwa rzuty trójścienną kostką,
- `D12-1`: wykonaj pojedynczy rzut kostką D12 i odejmij 1 od wyniku.

## Funkcjonalności

Program zawiera funkcję, która:
1. Przyjmuje kod rzutów jako parametr w postaci ciągu znaków.
2. Rozpoznaje i wyodrębnia informacje o:
   - typie kostki,
   - liczbie rzutów,
   - modyfikatorze.
3. Sprawdza poprawność kodu, zwracając komunikat o błędzie w przypadku niepoprawnego formatu.
4. Symuluje rzuty kostką i zwraca wynik.

## Obsługiwane typy kostek

Program obsługuje poniższe rodzaje kostek:
- `D3`, `D4`, `D6`, `D8`, `D10`, `D12`, `D20`, `D100`


##Wymagania
    Python 3.x