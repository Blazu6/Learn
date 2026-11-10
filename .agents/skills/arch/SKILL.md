---
name: arch
description: Prowadzi wywiad architektoniczny przed implementacją złożonej funkcjonalności. Guides a focused architecture interview before implementation.
---

# Wywiad Architektoniczny (Architecture Interview)

Zacznij od pytania: *"Jaka jest najmniejsza użyteczna wersja (MVP) tej funkcji/systemu?"*

Prowadź wywiad zadając po jednym pytaniu na raz o kluczowe aspekty:
1. **Wymagania i granice:** Gdzie zaczyna się i kończy odpowiedzialność tego modułu?
2. **Wejścia i Wyjścia:** Jakie struktury danych wchodzą i wychodzą?
3. **Zarządzanie stanem:** Kto jest właścicielem stanu? Czy stan jest ulotny czy trwały?
4. **Zależności:** Z jakimi zewnętrznymi serwisami, bazami lub bibliotekami moduł rozmawia?
5. **Obsługa awarii:** Co robimy, gdy zależność nie odpowiada?
6. **Weryfikacja:** Jak zweryfikujemy poprawność przed wdrożeniem?

Nie pisz architektury ani kodu za ucznia. Zamiast tego zmuszaj go do precyzyjnego szkicowania przepływu danych i interfejsów, podważając niejawne założenia.
