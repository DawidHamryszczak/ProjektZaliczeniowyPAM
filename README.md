# Countries App 🌍

Projekt zaliczeniowy stworzony w technologii Flutter. Aplikacja umożliwia przeglądanie informacji o krajach świata, oferując bogate możliwości filtrowania, wyszukiwania oraz pełną obsługę trybu offline.

## 🚀 Główne funkcjonalności

* **Przeglądanie krajów:** Lista państw z flagami, nazwami i stolicami.
* **Szczegóły państwa:** Widok detali zawierający populację, region, walutę, języki oraz link do Map Google.
* **Filtrowanie po regionach:** Dynamiczne pobieranie danych dla kontynentów (Europa, Azja, Afryka itp.) – obsługa wielu endpointów API.
* **Wyszukiwarka:** Filtrowanie wyników w czasie rzeczywistym.
* **System Ulubionych:** Możliwość dodawania i usuwania krajów z listy ulubionych.
* **Tryb Offline (Persystencja):** Aplikacja automatycznie zapisuje pobrane dane i umożliwia korzystanie z nich bez dostępu do internetu.

## 📡 Wykorzystane API

Aplikacja korzysta z publicznego API **REST Countries**.

* **Adres API:** [https://restcountries.com/](https://restcountries.com/)
* **Wykorzystane zapytania:**
    * `GET /v3.1/all` – Pobieranie listy wszystkich krajów.
    * `GET /v3.1/region/{region}` – Pobieranie krajów z konkretnego regionu.

## 🛠️ Instrukcja uruchomienia

Aby uruchomić projekt, upewnij się, że masz zainstalowane Flutter SDK oraz skonfigurowany emulator lub urządzenie fizyczne.

1.  **Pobierz zależności:**
    W terminalu w głównym katalogu projektu wpisz:
    ```bash
    flutter pub get
    ```

2.  **Uruchom aplikację:**
    ```bash
    flutter run
    ```

## 📱 Wspierane platformy

Projekt został przygotowany i przetestowany głównie na platformę:
* **Android** (Min SDK: 21)

*(Kod źródłowy jest kompatybilny z iOS, jednak konfiguracja uprawnień w pliku Info.plist nie była częścią tego zadania).*

## 📦 Wykorzystane biblioteki

* `provider` – Zarządzanie stanem aplikacji (MVVM).
* `http` – Komunikacja z API REST.
* `shared_preferences` – Zapisywanie danych lokalnie (Tryb Offline).
* `cached_network_image` – Optymalizacja i cache'owanie flag.
* `url_launcher` – Otwieranie linków do Map Google.
