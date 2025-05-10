## Blok 1: Fundamenty Azure i Python dla Danych (Szacowany czas: 3 miesiące)

**Cel bloku:** Zrozumienie ekosystemu Azure, umiejętność pracy z podstawowymi usługami danych, swobodne operowanie na danych w Pythonie przy użyciu Pandas, rozpoczęcie ścieżki DP-203. Pierwsze skrypty automatyzujące proste zadania na danych i integracje.

**Projekt bloku:** Zbudowanie prostego pipeline'u ETL w Pythonie, który pobiera dane z różnych źródeł (np. pliki CSV, API), transformuje je przy użyciu Pandas i ładuje do Azure SQL Database. Automatyzacja uruchamiania skryptu.

---

### Tydzień 1

**Cel tygodnia:** Zapoznanie się z podstawowymi koncepcjami chmury Azure, usługami danych oraz konfiguracja środowiska Python do pracy z danymi. Zbudowanie pierwszego prostego skryptu w Pythonie.

**Inspiracja:**
*Designing Your Life*: Zacznij od małych eksperymentów. Pierwszy tydzień to Twój prototyp – testuj, co działa, co sprawia trudność, dostosowuj.
*Mindset*: Pamiętaj, że każda nowa linijka kodu i każdy poznany serwis Azure to krok naprzód, nawet jeśli początkowo wydaje się skomplikowany.


| Nr dnia | Dzień tyg. | Azure | Python | Dokumentacja/Notatki | Propozycja uzupełniająca | Nauka języka | Ukończone? |
| :-- | :-- | :-- | :-- | :-- | :-- | :-- | :-- |
| 1 | 1 | [Wprowadzenie do data engineering w Azure (Moduł 1)](https://learn.microsoft.com/en-us/training/paths/get-started-data-engineering/) | [Instalacja Pythona i środowiska wirtualnego, podstawy składni](https://docs.python.org/3/tutorial/interpreter.html) | [Jak efektywnie robić notatki z kursów online w Notion](https://www.notion.so/help/guides/take-notes) | [Dodatkowy kurs Python dla początkujących na YouTube](https://www.youtube.com/watch?v=rfscVS0vtbw) | Czytanie dokumentacji Azure po angielsku | [ ] |
| 2 | 2 | [Przegląd Azure Portal i podstawowych zasobów](https://learn.microsoft.com/pl-pl/azure/azure-portal/azure-portal-overview) | [Praca z typami danych w Pythonie, operatory, instrukcje warunkowe](https://docs.python.org/3/tutorial/introduction.html) | [Jak tworzyć przejrzyste repozytoria na GitHub](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories) | [Interaktywne ćwiczenia Python na platformie Codecademy (część darmowa)](https://www.codecademy.com/learn/learn-python-3) | Słuchanie podcastu o Azure po angielsku | [ ] |
| 3 | 3 | [Azure Storage: Wprowadzenie do Blob Storage i Data Lake Storage Gen2](https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction) | [Pętle w Pythonie, funkcje, podstawy pracy z plikami (odczyt/zapis TXT, CSV)](https://docs.python.org/3/tutorial/controlflow.html) | [Jak pisać czytelne komentarze w kodzie Python](https://realpython.com/python-comments-guide/) | [Ćwiczenia z pisania funkcji w Pythonie na HackerRank](https://www.hackerrank.com/domains/python) | Oglądanie tutoriali Python po angielsku | [ ] |
| 4 | 4 | [Azure SQL Database: Tworzenie i zarządzanie bazą danych](https://learn.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview) | [Wprowadzenie do biblioteki Pandas: Series i DataFrame, wczytywanie danych z CSV](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html) | [Jak dokumentować schematy baz danych w Notion lub Draw.io](https://app.diagrams.net/) | [Kurs Pandas na Kaggle (darmowy)](https://www.kaggle.com/learn/pandas) | Czytanie dokumentacji Pandas po angielsku | [ ] |
| 5 | 5 | [Podstawy bezpieczeństwa w Azure: Role-Based Access Control (RBAC)](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview) | [Podstawowe operacje na DataFrame w Pandas: selekcja, filtrowanie, sortowanie](https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html) | [Jak prowadzić dziennik postępów w Notion z refleksjami (Metoda STAR)](https://www.notion.so/help/guides/weekly-agenda) | [Budowanie pierwszego prostego skryptu ETL (Extract-Transform-Load) w Pythonie z Pandas](https://www.youtube.com/watch?v=-br4F0s9fOY) | Podsumowanie tygodnia i planowanie po angielsku | [ ] |


---

**Projekt tygodnia:**
Stworzenie skryptu w Pythonie, który wczytuje dane z pliku CSV, wykonuje proste czyszczenie danych (np. usuwa puste wiersze, zmienia typy danych) przy użyciu biblioteki Pandas, a następnie zapisuje przetworzone dane do nowego pliku CSV. Umieszczenie kodu na GitHub z podstawowym plikiem README.md.

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:

* Zrozumienie podstawowych usług Azure Storage i SQL Database oraz umiejętność wczytywania i prostego manipulowania danymi w Pythonie przy użyciu biblioteki Pandas.

---

### Tydzień 2

**Cel tygodnia:** Pogłębienie wiedzy o usługach Azure Storage, wprowadzenie do Azure Data Factory jako narzędzia ETL oraz praktyczne wykorzystanie Pythona do interakcji z API i automatyzacji zadań.

**Inspiracja:**
*The Start-up of You*: Myśl o sobie jak o startupie – każdy projekt i nowa umiejętność to produkt, który rozwijasz. Inwestuj w "beta testy" swoich umiejętności poprzez małe projekty.
*Mindset*: Nie bój się "błędów kompilacji" czy problemów z konfiguracją. To naturalna część procesu nauki programowania i pracy z chmurą.


| Nr dnia | Dzień tyg. | Azure | Python | Dokumentacja/Notatki | Propozycja uzupełniająca | Nauka języka | Ukończone? |
| :-- | :-- | :-- | :-- | :-- | :-- | :-- | :-- |
| 6 | 1 | [Azure Data Lake Storage Gen2: Konfiguracja i zarządzanie](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) | [Praca z API w Pythonie: biblioteka `requests`, pobieranie danych JSON](https://realpython.com/python-requests/) | [Jak testować zapytania API za pomocą Postman/Insomnia](https://learning.postman.com/docs/getting-started/introduction/) | [Znajdź publiczne API (np. pogoda, giełda) i pobierz z niego dane do pliku CSV](https://github.com/public-apis/public-apis) | Czytanie dokumentacji `requests` po angielsku | [ ] |
| 7 | 2 | [Wprowadzenie do Azure Data Factory (ADF): Podstawowe komponenty, tworzenie pierwszego pipeline'u](https://learn.microsoft.com/en-us/azure/data-factory/introduction) | [Przetwarzanie danych JSON w Pythonie: biblioteka `json`, normalizacja danych zagnieżdżonych](https://realpython.com/python-json/) | [Jak wizualizować strukturę JSON online](https://jsonformatter.org/) | [Przetwórz złożony plik JSON i spłaszcz go do tabelarycznego formatu CSV używając Pandas](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.json_normalize.html) | Oglądanie tutoriali ADF po angielsku | [ ] |
| 8 | 3 | [ADF: Kopiowanie danych między różnymi źródłami (np. Blob Storage do Azure SQL)](https://learn.microsoft.com/en-us/azure/data-factory/copy-activity-overview) | [Obsługa błędów w Pythonie: bloki `try-except-finally`, własne wyjątki](https://docs.python.org/3/tutorial/errors.html) | [Dobre praktyki w obsłudze błędów w skryptach ETL](https://www.integrate.io/blog/error-handling-in-etl-pipelines/) | [Dodaj solidną obsługę błędów do swoich poprzednich skryptów Python](https://www.youtube.com/watch?v=6SPDvP9d6C8) | Pisanie komentarzy do kodu po angielsku | [ ] |
| 9 | 4 | [ADF: Podstawowe transformacje danych w przepływach danych (Mapping Data Flows)](https://learn.microsoft.com/en-us/azure/data-factory/concepts-data-flow-overview) | [Podstawy logowania w Pythonie: biblioteka `logging`, konfiguracja loggera](https://docs.python.org/3/howto/logging.html) | [Jak skonfigurować logowanie do pliku i na konsolę](https://realpython.com/python-logging/) | [Zaimplementuj logowanie zdarzeń (start, stop, błędy) w swoich skryptach ETL](https://docs.python.org/3/library/logging.handlers.html#rotatingfilehandler) | Czytanie blogów o Data Engineering po angielsku | [ ] |
| 10 | 5 | [ADF: Wyzwalacze (Triggers) – planowanie i uruchamianie pipeline'ów na żądanie](https://learn.microsoft.com/en-us/azure/data-factory/concepts-pipeline-execution-triggers) | [Pisanie funkcji i modułów w Pythonie: organizacja kodu, reużywalność](https://docs.python.org/3/tutorial/modules.html) | [Jak tworzyć moduły Pythona i używać ich w innych skryptach](https://realpython.com/python-modules-packages/) | [Zrefaktoryzuj swoje dotychczasowe skrypty, wydzielając powtarzalne fragmenty do funkcji i modułów](https://www.youtube.com/watch?v=CqvZ3vGoGs0) | Podsumowanie tygodnia i planowanie po angielsku | [ ] |


---

**Projekt tygodnia:**
Rozbudowa skryptu ETL z poprzedniego tygodnia: dane są pobierane z publicznego API (JSON), transformowane (czyszczenie, spłaszczanie struktury) i ładowane do Azure Data Lake Storage Gen2. Skrypt zawiera obsługę błędów i logowanie. Utworzenie prostego pipeline'u w Azure Data Factory, który uruchamia ten skrypt Pythona (np. przy użyciu Azure Custom Activity lub Azure Functions wywoływanych przez ADF).

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:

* Zrozumienie działania Azure Data Factory do orkiestracji zadań ETL oraz umiejętność pobierania i przetwarzania danych z API w Pythonie z obsługą błędów i logowaniem.
