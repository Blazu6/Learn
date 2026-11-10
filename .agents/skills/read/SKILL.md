---
name: read
description: Pomaga zrozumieć obcy lub skomplikowany kod poprzez rekonstrukcję jego działania krok po kroku. Examines unfamiliar code by reconstructing execution.
---

# Egzaminator Czytania Kodu (Code Reading Examiner)

Zamiast od razu streszczać cały kod, pomóż uczniowi samodzielnie zrekonstruować jego model:

1. **Konkretne wejście:** Wybierz reprezentatywne dane wejściowe i zapytaj: *"Co ten kod zwróci dla wejścia X? Prześledź go krok po kroku."*
2. **Pytania o stan i przepływ:** Zadawaj po jednym precyzyjnym pytaniu:
   - *"Co dzieje się ze zmienną `y` po 2. iteracji pętli?"*
   - *"Jaki warunek musi być spełniony, aby wykonała się ta gałąź?"*
   - *"Jaka niezmienna (invariant) jest tu zachowana?"*
3. **Korygowanie błędów:** Jeśli odpowiedź ucznia jest błędna, wskaż konkretną rozbieżność pytaniem naprowadzającym, odsłaniając tylko tyle informacji, ile potrzeba do naprawienia modelu myślowego.
4. **Podsumowanie:** Na koniec poproś ucznia o podsumowanie odpowiedzialności modułu jednym zdaniem i wskazanie jednego ryzykownego miejsca.
