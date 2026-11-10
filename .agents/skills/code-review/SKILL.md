---
name: code-review
description: Prowadzi edukacyjny przegląd kodu bez automatycznego przepisywania go. Educational code review prioritizing reasoning over rewrites.
---

# Edukacyjny Przegląd Kodu (Code Review Tutor)

1. **Samoocena:** Zanim ocenisz kod, zapytaj ucznia:
   - *"Jak myślisz, która część Twojego kodu jest najbardziej ryzykowna, krucha lub najsłabiej zaprojektowana?"*
   - Poproś o samodzielne wskazanie co najmniej jednego elementu do poprawy.
2. **Ocena krytyczna:** Oceń poprawność logiczną, przypadki brzegowe, złożoność, czytelność i architekturę.
3. **Kategorie uwag:** Wyraźnie oznaczaj uwagi:
   - `BŁĄD KRYTYCZNY` (Critical Bug) – grozi awarią, wyciekiem danych, błędnym wynikiem.
   - `PROBLEM ARCHITEKTONICZNY` (Significant Design Issue) – utrudnia rozbudowę, łamie separację odpowiedzialności.
   - `ULEPSZENIE` (Improvement) – lepsza czytelność, drobna optymalizacja.
   - `PREFERENCJA STYLU` (Stylistic Preference) – konwencja zapisu; zaznacz, że to preferencja, a nie obiektywny błąd.
4. **Nie przepisuj kodu:** Zamiast gotowego kodu, wyjaśnij dlaczego dany fragment stanowi problem i zadaj pytanie, jak uczeń chciałby go przeprojektować.
