# Blok 1: Fundamenty Azure i Python dla Danych (Szacowany czas: 3 miesiące)

**Cel bloku:** Zrozumienie ekosystemu Azure, umiejętność pracy z podstawowymi usługami danych, swobodne operowanie na danych w Pythonie przy użyciu Pandas, rozpoczęcie ścieżki DP-203. Pierwsze skrypty automatyzujące proste zadania na danych i integracje.

**Projekt bloku:** Zbudowanie prostego pipeline'u ETL w Pythonie, który pobiera dane z różnych źródeł (np. pliki CSV, API), transformuje je przy użyciu Pandas i ładuje do Azure SQL Database. Automatyzacja uruchamiania skryptu.

---

### Tydzień 1

**Cel tygodnia:** Zapoznanie się z podstawowymi koncepcjami chmury Azure, usługami danych oraz konfiguracja środowiska Python do pracy z danymi. Zbudowanie pierwszego prostego skryptu w Pythonie.

**Projekt tygodnia:**
Stworzenie skryptu w Pythonie, który wczytuje dane z pliku CSV, wykonuje proste czyszczenie danych (np. usuwa puste wiersze, zmienia typy danych) przy użyciu biblioteki Pandas, a następnie zapisuje przetworzone dane do nowego pliku CSV. Umieszczenie kodu na GitHub z podstawowym plikiem README.md.

**Inspiracja:**
*   *Designing Your Life*: Zacznij od małych eksperymentów. Pierwszy tydzień to Twój prototyp – testuj, co działa, co sprawia trudność, dostosowuj.
*   *Mindset*: Pamiętaj, że każda nowa linijka kodu i każdy poznany serwis Azure to krok naprzód, nawet jeśli początkowo wydaje się skomplikowany.
*   **Lektura:** Rozdział z "Mindset" Carol S. Dweck dotyczący różnicy między "fixed mindset" a "growth mindset".

| Nr dnia | Dzień tyg. | Azure                                                                                                                               | Python                                                                                                                          | Dokumentacja/Notatki                                                                                                   | Propozycja uzupełniająca                                                                                                    | Nauka języka                      | Ukończone? |
|---------|------------|-------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|-----------------------------------|------------|
| 1       | 1          | [Wprowadzenie do data engineering w Azure (Moduł 1)](https://learn.microsoft.com/en-us/training/paths/get-started-data-engineering/) | [Instalacja Pythona i środowiska wirtualnego, podstawy składni](https://docs.python.org/3/tutorial/interpreter.html)            | [Jak efektywnie robić notatki z kursów online w Notion](https://www.notion.so/help/guides/take-notes)                      | [Dodatkowy kurs Python dla początkujących na YouTube](https://www.youtube.com/watch?v=rfscVS0vtbw)                      | Czytanie dokumentacji Azure po angielsku | [ ]        |
| 2       | 2          | [Przegląd Azure Portal i podstawowych zasobów](https://learn.microsoft.com/pl-pl/azure/azure-portal/azure-portal-overview)               | [Praca z typami danych w Pythonie, operatory, instrukcje warunkowe](https://docs.python.org/3/tutorial/introduction.html)     | [Jak tworzyć przejrzyste repozytoria na GitHub](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories) | [Interaktywne ćwiczenia Python na platformie Codecademy (część darmowa)](https://www.codecademy.com/learn/learn-python-3) | Słuchanie podcastu o Azure po angielsku | [ ]        |
| 3       | 3          | [Azure Storage: Wprowadzenie do Blob Storage i Data Lake Storage Gen2](https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction) | [Pętle w Pythonie, funkcje, podstawy pracy z plikami (odczyt/zapis TXT, CSV)](https://docs.python.org/3/tutorial/controlflow.html) | [Jak pisać czytelne komentarze w kodzie Python](https://realpython.com/python-comments-guide/)                           | [Ćwiczenia z pisania funkcji w Pythonie na HackerRank](https://www.hackerrank.com/domains/python)                          | Oglądanie tutoriali Python po angielsku | [ ]        |
| 4       | 4          | [Azure SQL Database: Tworzenie i zarządzanie bazą danych](https://learn.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview) | [Wprowadzenie do biblioteki Pandas: Series i DataFrame, wczytywanie danych z CSV](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html) | [Jak dokumentować schematy baz danych w Notion lub Draw.io](https://app.diagrams.net/)                                 | [Kurs Pandas na Kaggle (darmowy)](https://www.kaggle.com/learn/pandas)                                                  | Czytanie dokumentacji Pandas po angielsku | [ ]        |
| 5       | 5          | [Podstawy bezpieczeństwa w Azure: Role-Based Access Control (RBAC)](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview) | [Podstawowe operacje na DataFrame w Pandas: selekcja, filtrowanie, sortowanie](https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html) | [Jak prowadzić dziennik postępów w Notion z refleksjami (Metoda STAR)](https://www.notion.so/help/guides/weekly-agenda) | [Budowanie pierwszego prostego skryptu ETL (Extract-Transform-Load) w Pythonie z Pandas](https://www.youtube.com/watch?v=-br4F0s9fOY) | Podsumowanie tygodnia i planowanie po angielsku | [ ]        |

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:
*   Zrozumienie podstawowych usług Azure Storage i SQL Database oraz umiejętność wczytywania i prostego manipulowania danymi w Pythonie przy użyciu biblioteki Pandas.

---

### Tydzień 2

**Cel tygodnia:** Pogłębienie wiedzy o usługach Azure Storage, wprowadzenie do Azure Data Factory jako narzędzia ETL oraz praktyczne wykorzystanie Pythona do interakcji z API i automatyzacji zadań.

**Projekt tygodnia:**
Rozbudowa skryptu ETL z poprzedniego tygodnia: dane są pobierane z publicznego API (JSON), transformowane (czyszczenie, spłaszczanie struktury) i ładowane do Azure Data Lake Storage Gen2. Skrypt zawiera obsługę błędów i logowanie. Utworzenie prostego pipeline'u w Azure Data Factory, który uruchamia ten skrypt Pythona (np. przy użyciu Azure Custom Activity lub Azure Functions wywoływanych przez ADF).

**Inspiracja:**
*   *The Start-up of You*: Myśl o sobie jak o startupie – każdy projekt i nowa umiejętność to produkt, który rozwijasz. Inwestuj w "beta testy" swoich umiejętności poprzez małe projekty.
*   *Mindset*: Nie bój się "błędów kompilacji" czy problemów z konfiguracją. To naturalna część procesu nauki programowania i pracy z chmurą.
*   **Lektura:** Rozdział z "The Start-up of You" Reida Hoffmana dotyczący budowania sieci kontaktów i znaczenia "słabych więzi".

| Nr dnia | Dzień tyg. | Azure                                                                                                                                  | Python                                                                                                                                 | Dokumentacja/Notatki                                                                                              | Propozycja uzupełniająca                                                                                                | Nauka języka                            | Ukończone? |
|---------|------------|----------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|------------|
| 6       | 1          | [Azure Data Lake Storage Gen2: Konfiguracja i zarządzanie](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction)        | [Praca z API w Pythonie: biblioteka `requests`, pobieranie danych JSON](https://realpython.com/python-requests/)                        | [Jak testować zapytania API za pomocą Postman/Insomnia](https://learning.postman.com/docs/getting-started/introduction/) | [Znajdź publiczne API (np. pogoda, giełda) i pobierz z niego dane do pliku CSV](https://github.com/public-apis/public-apis) | Czytanie dokumentacji `requests` po angielsku | [ ]        |
| 7       | 2          | [Wprowadzenie do Azure Data Factory (ADF): Podstawowe komponenty, tworzenie pierwszego pipeline'u](https://learn.microsoft.com/en-us/azure/data-factory/introduction) | [Przetwarzanie danych JSON w Pythonie: biblioteka `json`, normalizacja danych zagnieżdżonych](https://realpython.com/python-json/)              | [Jak wizualizować strukturę JSON online](https://jsonformatter.org/)                                                | [Przetwórz złożony plik JSON i spłaszcz go do tabelarycznego formatu CSV używając Pandas](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.json_normalize.html) | Oglądanie tutoriali ADF po angielsku      | [ ]        |
| 8       | 3          | [ADF: Kopiowanie danych między różnymi źródłami (np. Blob Storage do Azure SQL)](https://learn.microsoft.com/en-us/azure/data-factory/copy-activity-overview) | [Obsługa błędów w Pythonie: bloki `try-except-finally`, własne wyjątki](https://docs.python.org/3/tutorial/errors.html)                  | [Dobre praktyki w obsłudze błędów w skryptach ETL](https://www.integrate.io/blog/error-handling-in-etl-pipelines/)      | [Dodaj solidną obsługę błędów do swoich poprzednich skryptów Python](https://www.youtube.com/watch?v=6SPDvP9d6C8)           | Pisanie komentarzy do kodu po angielsku | [ ]        |
| 9       | 4          | [ADF: Podstawowe transformacje danych w przepływach danych (Mapping Data Flows)](https://learn.microsoft.com/en-us/azure/data-factory/concepts-data-flow-overview) | [Podstawy logowania w Pythonie: biblioteka `logging`, konfiguracja loggera](https://docs.python.org/3/howto/logging.html)                    | [Jak skonfigurować logowanie do pliku i na konsolę](https://realpython.com/python-logging/)                             | [Zaimplementuj logowanie zdarzeń (start, stop, błędy) w swoich skryptach ETL](https://docs.python.org/3/library/logging.handlers.html#rotatingfilehandler) | Czytanie blogów o Data Engineering po angielsku | [ ]        |
| 10      | 5          | [ADF: Wyzwalacze (Triggers) – planowanie i uruchamianie pipeline'ów na żądanie](https://learn.microsoft.com/en-us/azure/data-factory/concepts-pipeline-execution-triggers) | [Pisanie funkcji i modułów w Pythonie: organizacja kodu, reużywalność](https://docs.python.org/3/tutorial/modules.html)                   | [Jak tworzyć moduły Pythona i używać ich w innych skryptach](https://realpython.com/python-modules-packages/)            | [Zrefaktoryzuj swoje dotychczasowe skrypty, wydzielając powtarzalne fragmenty do funkcji i modułów](https://www.youtube.com/watch?v=CqvZ3vGoGs0) | Podsumowanie tygodnia i planowanie po angielsku | [ ]        |

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:
*   Zrozumienie działania Azure Data Factory do orkiestracji zadań ETL oraz umiejętność pobierania i przetwarzania danych z API w Pythonie z obsługą błędów i logowaniem.

---

---


### Tydzień 3

**Cel tygodnia:** Praktyczne wykorzystanie Azure Data Factory do budowy bardziej złożonych przepływów danych, w tym parametryzacji i dynamicznego sterowania. Pogłębienie umiejętności programowania w Pythonie poprzez tworzenie własnych modułów i efektywne zarządzanie kodem.

**Projekt tygodnia:**
Stworzenie sparametryzowanego pipeline'u w Azure Data Factory, który przetwarza pliki z określonego folderu w Azure Blob Storage (nazwa folderu jako parametr), wykonuje transformacje zdefiniowane w skrypcie Python (wywoływanym przez ADF) i ładuje wyniki do innej lokalizacji w Blob Storage. Skrypt Python zorganizowany w moduły.

**Inspiracja:**
*   *Designing Your Life*: "Odyssey Plans" - zastanów się nad trzema różnymi wersjami swojej kariery za 5 lat. Jakie małe kroki możesz zrobić w tym tygodniu, by przetestować te wizje?
*   *Mindset*: "Embrace challenges" - Potraktuj debugowanie skomplikowanego pipeline'u ADF lub modułu Pythona jako wyzwanie, które wzmocni Twoje umiejętności rozwiązywania problemów.
*   **Lektura:** Rozdział z "Mindset" Carol S. Dweck dotyczący różnicy między "fixed mindset" a "growth mindset".

| Nr dnia | Dzień tyg. | Azure                                                                                                                                                           | Python                                                                                                                                 | Dokumentacja/Notatki                                                                                                      | Propozycja uzupełniająca                                                                                                            | Nauka języka                            | Ukończone? |
|---------|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|------------|
| 11      | 1          | [ADF: Parametryzacja pipeline'ów i zestawów danych](https://learn.microsoft.com/en-us/azure/data-factory/control-flow-expression-language-functions#parameters)       | [Tworzenie własnych modułów w Pythonie, importowanie modułów](https://docs.python.org/3/tutorial/modules.html#packages)                     | [Jak strukturyzować projekty Pythona z wieloma modułami](https://realpython.com/python-application-layouts/)                 | [Przeanalizuj strukturę popularnej biblioteki Python na GitHub (np. `requests` lub `pandas`)](https://github.com/psf/requests) | Czytanie o "parameterization" po angielsku | [ ]        |
| 12      | 2          | [ADF: Używanie zmiennych i wyrażeń w pipeline'ach](https://learn.microsoft.com/en-us/azure/data-factory/control-flow-system-variables)                                  | [Praca z systemem plików w Pythonie: moduł `os`, `pathlib`](https://docs.python.org/3/library/os.path.html)                           | [Jak debugować pipeline'y w Azure Data Factory](https://learn.microsoft.com/en-us/azure/data-factory/control-flow-debug) | [Napisz skrypt Pythona, który listuje pliki w folderze i filtruje je po rozszerzeniu](https://www.pythonforbeginners.com/os/pythons-os-module) | Oglądanie tutoriali o "expressions" w ADF | [ ]        |
| 13      | 3          | [ADF: Działania kontroli przepływu (ForEach, If Condition, Switch)](https://learn.microsoft.com/en-us/azure/data-factory/control-flow-activities-overview)            | [Zaawansowane funkcje w Pythonie: `*args`, `**kwargs`, funkcje lambda](https://realpython.com/python-kwargs-and-args/)                   | [Dobre praktyki pisania reużywalnych funkcji Pythona](https://docs.python-guide.org/writing/style/)                         | [Przepisz istniejącą funkcję Pythona używając `*args` i `**kwargs` dla większej elastyczności](https://www.geeksforgeeks.org/args-kwargs-python/) | Pisanie dokumentacji funkcji po angielsku | [ ]        |
| 14      | 4          | [ADF: Wywoływanie skryptów Pythona (np. przez Azure Batch lub Custom Activity)](https://learn.microsoft.com/en-us/azure/data-factory/transform-data-using-python)        | [Konfiguracja i używanie środowisk wirtualnych (`venv`) dla projektów Pythona](https://docs.python.org/3/library/venv.html)              | [Zarządzanie zależnościami w Pythonie za pomocą `requirements.txt`](https://pip.pypa.io/en/stable/cli/pip_freeze/)        | [Stwórz nowy projekt Pythona z własnym środowiskiem wirtualnym i plikiem `requirements.txt`](https://www.youtube.com/watch?v=KXVCP6L4gC8) | Czytanie o "virtual environments" | [ ]        |
| 15      | 5          | [ADF: Monitorowanie i zarządzanie uruchomieniami pipeline'ów](https://learn.microsoft.com/en-us/azure/data-factory/monitor-visually)                                  | [Refaktoryzacja kodu Pythona: poprawa czytelności, wydajności, eliminacja powtórzeń](https://refactoring.guru/refactoring/what-is-refactoring) | [Narzędzia do statycznej analizy kodu Python (np. Pylint, Flake8)](https://realpython.com/python-linters-code-quality/) | [Użyj Pylint lub Flake8 do analizy swoich dotychczasowych skryptów i popraw zidentyfikowane problemy](https://pylint.pycqa.org/en/latest/tutorial.html) | Podsumowanie tygodnia i planowanie po angielsku | [ ]        |

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:
*   Umiejętność budowania sparametryzowanych i sterowanych dynamicznie pipeline'ów w Azure Data Factory oraz organizowania kodu Pythona w reużywalne moduły.

---

### Tydzień 4

**Cel tygodnia:** Skupienie na pracy z Azure SQL Database, w tym bardziej zaawansowane operacje i integracja z Pythonem. Wprowadzenie do koncepcji ORM.

**Projekt tygodnia:**
Stworzenie skryptu Pythona, który wykorzystuje bibliotekę `pyodbc` (lub wprowadzenie do SQLAlchemy) do wykonywania operacji CRUD (Create, Read, Update, Delete) na tabelach w Azure SQL Database. Skrypt powinien być sparametryzowany i zawierać obsługę transakcji.

**Inspiracja:**
*   *Designing Your Life*: "Brainstorming" - poświęć czas na wygenerowanie wielu pomysłów na projekty lub rozwiązania problemów, zanim wybierzesz jeden. Nie oceniaj pomysłów na tym etapie.
*   *Mindset*: "Seek feedback" - Nawet jeśli pracujesz samodzielnie, szukaj sposobów na uzyskanie informacji zwrotnej (np. publikując fragmenty kodu na forach, porównując swoje rozwiązania z innymi).
*   **Lektura:** Rozdział z "The Start-up of You" Reida Hoffmana dotyczący budowania sieci kontaktów i znaczenia "słabych więzi".

| Nr dnia | Dzień tyg. | Azure                                                                                                                              | Python                                                                                                                               | Dokumentacja/Notatki                                                                                                | Propozycja uzupełniająca                                                                                                   | Nauka języka                               | Ukończone? |
|---------|------------|------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|------------|
| 16      | 1          | [Azure SQL Database: Zaawansowane typy danych, indeksy, klucze](https://learn.microsoft.com/en-us/sql/relational-databases/tables/tables?view=sql-server-ver16) | [Praca z bazami danych w Pythonie z `pyodbc`: nawiązywanie połączenia, wykonywanie zapytań](https://github.com/mkleehammer/pyodbc/wiki/Cursor) | [Jak pisać bezpieczne zapytania SQL (unikanie SQL Injection)](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html) | [Przeanalizuj schemat istniejącej bazy danych i zidentyfikuj potencjalne optymalizacje indeksów](https://www.red-gate.com/simple-talk/databases/sql-server/learn/sql-server-index-basics/) | Czytanie o "database indexing" po angielsku | [ ]        |
| 17      | 2          | [Azure SQL Database: Procedury składowane, funkcje, wyzwalacze (wprowadzenie)](https://learn.microsoft.com/en-us/sql/relational-databases/stored-procedures/stored-procedures-database-engine?view=sql-server-ver16) | [Wykonywanie zapytań typu INSERT, UPDATE, DELETE z `pyodbc`](https://github.com/mkleehammer/pyodbc/wiki/Calling-Stored-Procedures)          | [Zarządzanie transakcjami w `pyodbc` (commit, rollback)](https://github.com/mkleehammer/pyodbc/wiki/Transactions)      | [Napisz skrypt Pythona, który dodaje, modyfikuje i usuwa rekordy w tabeli testowej Azure SQL](https://www.sqlshack.com/python-scripts-to-insert-update-and-delete-data-in-sql-server/) | Oglądanie tutoriali o "stored procedures" | [ ]        |
| 18      | 3          | [Azure SQL Database: Zarządzanie transakcjami i poziomami izolacji (wprowadzenie)](https://learn.microsoft.com/en-us/sql/relational-databases/sql-server-transaction-locking-and-row-versioning-guide?view=sql-server-ver16) | [Wprowadzenie do ORM (Object-Relational Mapping) z SQLAlchemy: definicja modeli, sesje](https://docs.sqlalchemy.org/en/14/orm/tutorial.html) | [Porównanie `pyodbc` vs SQLAlchemy: kiedy używać którego?](https://www.geeksforgeeks.org/sqlalchemy-vs-pyodbc/)         | [Zdefiniuj prosty model danych w SQLAlchemy i wykonaj podstawowe operacje na bazie](https://www.compose.com/articles/using-postgresql-through-sqlalchemy/) | Pisanie zapytań SQL po angielsku        | [ ]        |
| 19      | 4          | [Azure SQL Database: Import i eksport danych (np. BACPAC, narzędzia)](https://learn.microsoft.com/en-us/azure/azure-sql/database/database-export)           | [Wykonywanie zapytań SELECT z SQLAlchemy ORM, filtrowanie, sortowanie](https://docs.sqlalchemy.org/en/14/orm/query.html)                     | [Jak tworzyć migracje schematu bazy danych (np. z Alembic dla SQLAlchemy)](https://alembic.sqlalchemy.org/en/latest/tutorial.html) | [Zaimplementuj migrację schematu dla swojego modelu SQLAlchemy przy użyciu Alembic](https://testdriven.io/blog/fastapi-alembic/) | Czytanie o "ORM benefits" po angielsku    | [ ]        |
| 20      | 5          | [Azure SQL Database: Monitorowanie wydajności (Query Performance Insight)](https://learn.microsoft.com/en-us/azure/azure-sql/database/query-performance-insight-use) | [Praktyczne zastosowanie SQLAlchemy ORM w projekcie: operacje CRUD na modelu](https://www.learndatasci.com/tutorials/using-databases-python-sqlalchemy/) | [Jak dokumentować modele danych i relacje w Notion/Draw.io](https://app.diagrams.net/)                              | [Rozbuduj swój skrypt z `pyodbc` o dodatkowe funkcje lub przepisz go używając SQLAlchemy](https://www.youtube.com/watch?v=woKYyhLCcnU) | Podsumowanie tygodnia i planowanie po angielsku | [ ]        |

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:
*   Efektywna praca z Azure SQL Database z poziomu Pythona, w tym wykonywanie operacji CRUD i zrozumienie podstaw ORM z SQLAlchemy.

---

### Tydzień 5

**Cel tygodnia:** Zrozumienie i implementacja podstawowych mechanizmów bezpieczeństwa w Azure oraz wprowadzenie do testowania kodu Python i zaawansowanych funkcji Git/GitHub.

**Projekt tygodnia:**
Zabezpieczenie dostępu do Azure SQL Database przy użyciu Azure Active Directory Authentication. Stworzenie zestawu testów jednostkowych dla kluczowych funkcji w istniejącym projekcie Pythona (np. z poprzednich tygodni) przy użyciu biblioteki `unittest` lub `pytest`. Wykorzystanie gałęzi (branches) i pull requestów na GitHub do zarządzania zmianami w projekcie.

**Inspiracja:**
*   *Designing Your Life*: "Failure Reframe" - Przeanalizuj "porażkę" lub błąd z tego tygodnia (np. problem z konfiguracją bezpieczeństwa, niepoprawny test) i zastanów się, czego się dzięki temu nauczyłeś.
*   *Mindset*: "Effort is key" - Pamiętaj, że wysiłek włożony w naukę pisania testów czy konfigurację bezpieczeństwa zaprocentuje w przyszłości mniejszą liczbą błędów i stabilniejszymi rozwiązaniami.
*   **Lektura:** Fragmenty z "Clean Code" Roberta C. Martina dotyczące pisania testowalnego kodu i znaczenia testów.

| Nr dnia | Dzień tyg. | Azure                                                                                                                                                              | Python                                                                                                                                 | Dokumentacja/Notatki                                                                                                   | Propozycja uzupełniająca                                                                                                    | Nauka języka                                 | Ukończone? |
|---------|------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|----------------------------------------------|------------|
| 21      | 1          | [Azure Security Center: Przegląd funkcji, rekomendacje bezpieczeństwa](https://learn.microsoft.com/en-us/azure/security-center/security-center-introduction)            | [Wprowadzenie do testowania w Pythonie: biblioteka `unittest`](https://docs.python.org/3/library/unittest.html)                          | [Jak pisać dobre testy jednostkowe: zasady FIRST](https://medium.com/@pjbgf/first-principle-of-testing-c1b03500f1a)           | [Napisz pierwsze testy jednostkowe dla prostej funkcji Pythona](https://realpython.com/python-testing/)                       | Czytanie o "security best practices" w Azure | [ ]        |
| 22      | 2          | [Azure Key Vault: Zarządzanie sekretami, kluczami, certyfikatami (wprowadzenie)](https://learn.microsoft.com/en-us/azure/key-vault/general/overview)                   | [Alternatywa dla `unittest`: biblioteka `pytest`, podstawowe użycie](https://docs.pytest.org/en/stable/getting-started.html)               | [Porównanie `unittest` vs `pytest`](https://stackoverflow.com/questions/2048083/unittest-vs-pytest)                       | [Przepisz testy z `unittest` na `pytest` lub napisz nowe używając `pytest`](https://www.youtube.com/watch?v=LteNqj4DFgE)     | Oglądanie tutoriali o Azure Key Vault         | [ ]        |
| 23      | 3          | [Uwierzytelnianie w Azure SQL Database: SQL Authentication vs Azure AD Authentication](https://learn.microsoft.com/en-us/azure/azure-sql/database/authentication-aad-overview) | [Testowanie kodu, który operuje na plikach lub zewnętrznych zasobach: mocking z `unittest.mock`](https://docs.python.org/3/library/unittest.mock.html) | [Jak efektywnie używać mocków w testach](https://realpython.com/python-mock-library/)                                  | [Napisz testy dla funkcji Pythona, która odczytuje dane z pliku, używając mockowania](https://testdriven.io/blog/python-mocking-examples/) | Pisanie scenariuszy testowych po angielsku     | [ ]        |
| 24      | 4          | [Role-Based Access Control (RBAC) w Azure: Przypisywanie ról, niestandardowe role (wprowadzenie)](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview) | [Git i GitHub: Praca z gałęziami (branching, merging)](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)   | [Model przepływu pracy Gitflow (wprowadzenie)](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) | [Stwórz nową gałąź na GitHub, wprowadź zmiany i zrób pull request do gałęzi głównej](https://www.youtube.com/watch?v=RGOj5yH7evk) | Czytanie o "git branching strategies"       | [ ]        |
| 25      | 5          | [Azure Policy: Wymuszanie standardów i zgodności (wprowadzenie)](https://learn.microsoft.com/en-us/azure/governance/policy/overview)                                 | [Git i GitHub: Pull Requests, code review (podstawy)](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) | [Jak przeprowadzać efektywne code review](https://google.github.io/eng-practices/review/reviewer/)                       | [Przejrzyj pull request innego projektu open-source lub poproś kogoś o review Twojego kodu](https://www.conventionalcommits.org/en/v1.0.0/) | Podsumowanie tygodnia i planowanie po angielsku | [ ]        |

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:
*   Zrozumienie podstawowych koncepcji bezpieczeństwa w Azure oraz umiejętność pisania testów jednostkowych w Pythonie i efektywnej pracy z systemem kontroli wersji Git.

---

### Tydzień 6

**Cel tygodnia:** Skupienie się na monitorowaniu zasobów w Azure oraz optymalizacji kodu Pythona pod kątem wydajności i czytelności, z wykorzystaniem dobrych praktyk programistycznych.

**Projekt tygodnia:**
Zintegrowanie Azure Monitor z istniejącą aplikacją/skryptem Pythona w celu zbierania metryk i logów. Przeprowadzenie refaktoryzacji wybranego skryptu Pythona w celu poprawy jego wydajności (np. przez profilowanie) i zgodności z zasadami PEP 8.

**Inspiracja:**
*   *Designing Your Life*: "Prototyping Conversations" - Porozmawiaj z kimś, kto już pracuje jako Azure Data Engineer. Zapytaj o typowe problemy z wydajnością, monitorowaniem, jakie narzędzia są kluczowe.
*   *Mindset*: "Learn from criticism" - Jeśli narzędzie do analizy kodu (linter) lub profiler wskaże obszary do poprawy, potraktuj to jako cenną informację zwrotną, a nie krytykę.
*   **Lektura:** Rozdział z "Pragmatic Programmer" Andrew Hunta i Davida Thomasa dotyczący pisania kodu, który jest łatwy do zmiany ("Don't Live with Broken Windows", "DRY - Don't Repeat Yourself").

| Nr dnia | Dzień tyg. | Azure                                                                                                                                          | Python                                                                                                                                | Dokumentacja/Notatki                                                                                                   | Propozycja uzupełniająca                                                                                                  | Nauka języka                                   | Ukończone? |
|---------|------------|------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|------------|
| 26      | 1          | [Azure Monitor: Wprowadzenie, zbieranie metryk i logów](https://learn.microsoft.com/en-us/azure/azure-monitor/overview)                           | [Optymalizacja kodu Pythona: Podstawowe techniki, unikanie typowych pułapek](https://wiki.python.org/moin/PythonSpeed/PerformanceTips) | [Jak czytać i interpretować metryki wydajności w Azure Monitor](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/data-platform-metrics) | [Przeanalizuj metryki dla jednej z Twoich usług Azure (np. SQL Database)](https://www.youtube.com/watch?v=1qZ3z0Q9Z3w)     | Czytanie o "performance metrics" w Azure       | [ ]        |
| 27      | 2          | [Azure Log Analytics: Tworzenie zapytań Kusto Query Language (KQL) - wprowadzenie](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-tutorial) | [Profilowanie kodu Pythona: moduł `cProfile`, `profile`](https://docs.python.org/3/library/profile.html)                           | [Narzędzia do wizualizacji wyników profilowania (np. snakeviz)](https://jiffyclub.github.io/snakeviz/)                  | [Sprawdź wydajność swojego skryptu Pythona używając `cProfile` i `snakeviz`](https://www.youtube.com/watch?v=m_a0fN4jHGU) | Oglądanie tutoriali o KQL                     | [ ]        |
| 28      | 3          | [Azure Alerts: Konfiguracja alertów na podstawie metryk i logów](https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-overview)    | [Dobre praktyki programistyczne w Pythonie: PEP 8, czytelność kodu, komentarze](https://peps.python.org/pep-0008/)                     | [Automatyczne formatowanie kodu (np. Black, autopep8)](https://github.com/psf/black)                                  | [Użyj Black lub autopep8 do sformatowania swojego kodu Pythona zgodnie z PEP 8](https://realpython.com/python-code-quality/) | Pisanie zapytań KQL po angielsku              | [ ]        |
| 29      | 4          | [Application Insights (dla aplikacji): Wprowadzenie, integracja z Pythonem (opcjonalnie)](https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview) | [Pisanie dokumentacji kodu Pythona: docstringi, narzędzia (np. Sphinx - wprowadzenie)](https://www.python.org/dev/peps/pep-0257/)         | [Standardy pisania docstringów (Google, NumPy, reStructuredText)](https://stackoverflow.com/questions/3898572/what-is-the-standard-python-docstring-format) | [Dodaj docstringi do wszystkich funkcji i modułów w swoim projekcie](https://www.youtube.com/watch?v=1i_nC4e9y1Y)          | Czytanie o "application monitoring" po angielsku | [ ]        |
| 30      | 5          | [Dashboardy w Azure Portal: Wizualizacja metryk i logów](https://learn.microsoft.com/en-us/azure/azure-portal/azure-portal-dashboards)           | [Refaktoryzacja skryptu Pythona na podstawie wyników profilowania i zasad czystego kodu](https://refactoring.guru/catalog)              | [Przykłady refaktoryzacji w Pythonie](https://github.com/rasbt/python_reference/blob/master/refactoring/refactoring_examples.ipynb) | [Wybierz jeden ze swoich skryptów i przeprowadź jego pełną refaktoryzację](https://www.youtube.com/watch?v=DZyWN76C_c0)    | Podsumowanie tygodnia i planowanie po angielsku | [ ]        |

---

**Podsumowanie tygodnia:**
Najważniejsza nowa umiejętność:
*   Monitorowanie zasobów Azure przy użyciu Azure Monitor i Log Analytics oraz umiejętność optymalizacji i refaktoryzacji kodu Pythona zgodnie z dobrymi praktykami.

---
