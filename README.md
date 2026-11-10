# 🧠 AI Learning Toolkit (Wersja dla Google Antigravity)

> Zainspirowane rozwiązaniem [Manware](https://www.youtube.com/watch?v=JDIXhJX6kdE) – skonfigurowane natywnie dla środowiska **Google Antigravity**.

Zestaw reguł, umiejętności (skills) i agentów, który zamienia sztuczną inteligencję z **„maszyny do generowania kodu”** w **prywatnego mentora, recenzenta i partnera w myśleniu sokratejskim**.

---

## 🎯 Główna Idea

```text
Twoja próba ➔ Twoja hipoteza/predykcja ➔ Minimalna podpowiedź AI ➔ Własna implementacja ➔ Testy ➔ Wyjaśnienie ➔ Edukacyjny przegląd ➔ Powtórka z odstępami
```

**Złota zasada:** AI nigdy nie podaje rozwiązania na tacy jako pierwsze. AI zmusza Cię do myślenia, przewidywania i stawiania hipotez. Im więcej samodzielnego wysiłku umysłowego włożysz, tym szybciej i trwalej opanujesz programowanie.

---

## 🚀 Jak z tego korzystać w Antigravity?

Ten folder (`CodingLearn`) jest już w pełni skonfigurowany pod Google Antigravity:
- W katalogu głównym znajduje się reguła **`GEMINI.md`**, która sprawia, że w każdej rozmowie w tym katalogu agent domyślnie przyjmuje rolę **Towarzysza Nauki (Learning Companion)**.
- W `.agents/skills/` znajduje się **15 wyspecjalizowanych modułów/umiejętności**.
- W `.agents/agents/` znajdują się **4 dedykowani agenci edukacyjni**.
- W katalogu `learning/` masz gotowe szablony dziennika wiedzy.

### Rozpoczęcie sesji:
Wystarczy, że napiszesz na czacie w naturalny sposób po polsku, np.:
- *"Chcę się nauczyć pętli w Pythonie"* ➔ Agent uruchomi tryb `study` i poprowadzi Cię krok po kroku.
- *"Utknąłem na zadaniu ze strukturami danych, podpowiedz mi"* ➔ Agent uruchomi drabinę podpowiedzi `hint`.
- *"Mój kod rzuca błąd IndexError, pomóż mi zrozumieć dlaczego"* ➔ Agent uruchomi procedurę `debug`.
- *"Sprawdź mój kod i powiedz co mogę poprawić"* ➔ Agent uruchomi `code-review`.
- *"Chcę sprawdzić, czy naprawdę rozumiem mechanizm asynchroniczności (async/await)"* ➔ Agent uruchomi test Feynmana `explain`.

---

## 🪜 Drabina Podpowiedzi (Hint Ladder) – Serce Toolkitu

Gdy utkniesz, agent nie rzuca w Ciebie gotowym blokiem kodu. Schodzi po drabinie od najmniejszej interwencji:

| Poziom | Nazwa | Co robi AI? |
| :---: | :--- | :--- |
| **0** | **Tylko pytanie** | Zadaje pytanie sokratejskie zmuszające do spojrzenia na właściwy element. |
| **1** | **Kierunek** | Wskazuje pojęcie, funkcję, moduł lub stronę dokumentacji do przeczytania. |
| **2** | **Wskazówka pojęciowa** | Tłumaczy ogólny mechanizm (np. czym jest mutowalność), bez podawania odpowiedzi. |
| **3** | **Wskazówka strategiczna**| Podaje słowny plan/kroki algorytmiczne rozwiązania. |
| **4** | **Pseudokod** | Szkicuje ogólną strukturę w pseudokodzie (bez konkretnego języka). |
| **5** | **Częściowy kod** | Pokazuje jedną kluczową linijkę lub sygnaturę. |
| **6** | **Pełna implementacja** | Gotowy kod – **wyłącznie na Twoje wyraźne życzenie**. |

---

## 🛠️ Dostępne Tryby i Umiejętności (Workflows & Skills)

1. **`study` (Sesja nauki)** – Uniwersalny punkt startowy. Określasz, czego chcesz się nauczyć, a AI dobiera właściwy proces dydaktyczny.
2. **`hint` (Wskazówki)** – Stopniowane naprowadzanie na rozwiązanie krok po kroku.
3. **`debug` (Interaktywne debugowanie)** – AI pyta: czego oczekiwałeś, co się stało, jaka jest Twoja hipoteza i jaki najmniejszy test/log pozwoli to sprawdzić.
4. **`autopsy` (Sekcja zwłok błędu)** – Po usunięciu trudnego błędu analizujesz rozbieżność między pierwotnym wyobrażeniem a rzeczywistością, by błąd nigdy nie wrócił.
5. **`read` (Czytanie obcego kodu)** – Nauka analizy bibliotek lub cudzego kodu poprzez predykcję ("Co zwróci ta linia dla wejścia X?").
6. **`code-review` (Edukacyjny przegląd kodu)** – Zanim AI oceni kod, to Ty wskazujesz najsłabszy punkt. Uwagi dzielone są na błędy, architekturę i preferencje.
7. **`test` (Projektowanie testów)** – Formułowanie kontraktu i przypadków skrajnych przed napisaniem ani jednej linijki kodu właściwego.
8. **`explore` (Eksploracja kompromisów)** – Obrona obecnego rozwiązania i porównanie z realnymi alternatywami pod wpływem stres-testów (np. 10 mln rekordów, brak sieci).
9. **`arch` (Wywiad architektoniczny)** – Projektowanie MVP, granic odpowiedzialności, obsługi awarii i stanu przed kodowaniem.
10. **`explain` (Test Feynmana / Teach-back)** – Tłumaczysz zagadnienie tak, jakbyś uczył początkującego. AI wyłapuje żargon, luki myślowe i sprzeczności.
11. **`retrieve` (Spaced Retrieval)** – Krótka rozgrzewka przed kodowaniem z pytań predykcyjnych opartych na Twoim dzienniku wiedzy.
12. **`api` (Poznawanie API)** – 7 pytań fundamentów: po co powstało, jakie ma założenia, alternatywy, trade-offy i kiedy pod żadnym pozorem go NIE używać.

---

## 🤖 4 Dedykowanych Agentów

Możesz ich wywoływać w Antigravity, gdy potrzebujesz konkretnej perspektywy:

- **`learning-reviewer`**: Doświadczony Senior Developer, który nie przepisuje Twojego kodu, lecz uczy Cię myślenia o jakości i architekturze.
- **`learning-auditor`**: Skrupulatny audytor, który weryfikuje Twoje hipotezy, szuka luk w testach i przypadków brzegowych.
- **`learning-research`**: Pomocnik w zgłębianiu kodu źródłowego i dokumentacji z zachowaniem Twojego toku rozumowania.
- **`learning-browser`**: Asystent weryfikacji faktów w sieci i dokumentacji technicznej.

---

## 📓 Dziennik Nauki (`learning/`)

W katalogu `learning/` znajdują się 4 pliki:
- `learning/concepts.md` – trwałe pojęcia, modele myślowe i analogie.
- `learning/mistakes.md` – trudne błędy i nawyki zapobiegawcze.
- `learning/questions.md` – otwarte pytania, do których warto wrócić.
- `learning/review.md` – baza powtórek dla trybu `retrieve`.

---

## ⚡ Tryb Produkcyjny ("Shipping Mode")

Gdy przyjdzie moment, w którym nie chcesz się uczyć, tylko musisz szybko zrealizować zadanie komercyjne lub projektowe:
> Wystarczy napisać: **"ship this"**, **"daj mi gotowy kod"** lub **"tryb produkcyjny"**.

Wtedy agent natychmiast wyłącza rolę dydaktyczną i pisze kompletny, zoptymalizowany kod produkcyjny.
