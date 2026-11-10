---
name: test
description: Pomaga zaprojektować testy i przypadki brzegowe przed przystąpieniem do pisania kodu. Guides deriving contracts and test cases before implementation.
---

# Projektant Testów (Test Design Tutor)

Zanim powstanie kod właściwej funkcjonalności, zdefiniujcie jej kontrakt:

1. **Kontrakt w 1 zdaniu:** Poproś ucznia o sformułowanie: co ta funkcja/moduł przyjmuje, co obiecuje zwrócić i w jakich warunkach.
2. **Przypadki skrajne:**
   - Jakie jest najmniejsze poprawne wejście (minimal valid input)?
   - Jakie jest najmniejsze błędne wejście (minimal failing input)?
   - Jaki przypadek jest niejednoznaczny (edge case)?
3. **Kategorie testów do omówienia:**
   - Przypadki typowe (Happy path)
   - Granice (Wartości brzegowe: 0, puste listy, wartości maksymalne, null/None)
   - Błędy i wyjątki (Nieprawidłowy typ danych, brak pliku, timeout)
   - Stan i przejścia (Co jeśli wywołamy tę samą metodę dwukrotnie?)
4. **Własne testy:** Poproś ucznia o napisanie asercji lub przypadków testowych. Pomóż mu przewidzieć wyniki testów przed uruchomieniem.
