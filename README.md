# Moonbase Control: Guards

Zadanie z modułu Angular. Repozytorium zawiera kod startowy aplikacji Moonbase Control dla tej lekcji.

## Zadanie

Zabezpiecz ścieżkę szczegółów incydentu przed próbą otwarcia incydentu, który nie istnieje.

W aplikacji szczegóły incydentu są dostępne pod ścieżką zawierającą jego `id`. Użytkownik może jednak wejść bezpośrednio na adres wskazujący incydent, który został usunięty lub nigdy nie istniał.

Twoim zadaniem jest:

- Utworzyć funkcyjny guard sprawdzający, czy incydent o `id` znajdującym się w URL istnieje.
- Wykorzystać `HttpClient` do wykonania odpowiedniego zapytania do API.
- Pozwolić na aktywację ścieżki, jeśli incydent istnieje.
- W przypadku nieistniejącego incydentu przekierować użytkownika do listy incydentów.
- Wyświetlić za pomocą `MatSnackBar` informację, że wskazany incydent nie istnieje.
- Przypisać utworzony guard do ścieżki szczegółów incydentu za pomocą `canActivate`.
Rezultat: wejście na adres istniejącego incydentu otwiera jego szczegóły. Próba wejścia na adres z nieistniejącym `id` nie aktywuje widoku szczegółów — użytkownik otrzymuje komunikat i zostaje przekierowany do listy incydentów.

## Jak zacząć

1. Zrób fork tego repozytorium na swoje konto GitHub.
2. Sklonuj swój fork na komputer.
3. Zainstaluj zależności: `npm install`.
4. Uruchom aplikację: `npm start`.
5. Jeśli zadanie korzysta z danych z API, uruchom w drugim terminalu mock API: `npm run api`.

## Jak oddać zadanie

1. Zapisz zmiany w commicie i wypchnij je do swojego forka.
2. Otwórz Pull Request z forka do repozytorium `mate-academy/angular_route-guards`, do brancha `main`.
3. Platforma uruchomi review Twojego Pull Requesta.
