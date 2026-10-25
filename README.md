# Asystent-Sprzedawcy

Prywatne narzędzie do zarządzania **moim własnym** kontem sprzedawcy na Allegro. Nie jest udostępniane innym sprzedawcom i nie świadczy usług osobom trzecim.

## Co robi

- Odczytuje zamówienia, oferty, wiadomości od kupujących, dyskusje i reklamacje oraz dane o sprzedaży.
- Przygotowuje **propozycje** zmian: ceny i stany ofert, odpowiedzi do kupujących, numery przesyłek, edycję i wystawianie ofert, wyróżnienia, kody EAN i ustawienia sprzedaży.
- **Żadna zmiana nie jest wykonywana automatycznie.** Każdą propozycję sprzedawca przegląda i ręcznie zatwierdza przed wysłaniem do Allegro.

## Jak działa

- Aplikacja działa lokalnie, na komputerze sprzedawcy.
- Łączy się z [Allegro REST API](https://developer.allegro.pl/documentation) wyłącznie w imieniu właściciela konta, z autoryzacją OAuth2 typu *device flow*.
- Tokeny dostępu są przechowywane tylko lokalnie i nie są nigdzie przesyłane.
- Każde zapytanie do API zawiera identyfikator `User-Agent` w formacie wymaganym przez Allegro.
- Wykonane zmiany są zapisywane w lokalnym dzienniku, który nie zawiera danych osobowych kupujących.

## Dane

Aplikacja przetwarza tylko dane z konta właściciela, potrzebne do obsługi sprzedaży. Danych kupujących nie przekazuje osobom trzecim ani nie wykorzystuje do innych celów.

## Kontakt

Pytania dotyczące aplikacji: przez zakładkę [Issues](../../issues) w tym repozytorium.
