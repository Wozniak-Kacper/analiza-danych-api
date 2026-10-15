# Analiza danych z API JSONPlaceholder

Projekt pobiera dane z publicznego API JSONPlaceholder, oblicza podstawowe statystyki
i przedstawia wyniki na wykresach. Powstał jako zadanie rekrutacyjne.

**Demo:** [Otwórz notebook w Google Colab](https://colab.research.google.com/github/Wozniak-Kacper/analiza-danych-api/blob/main/analizaAPI.ipynb)

## Zrzuty ekranu

![Podsumowanie realizacji zadań](podsumowanie_realizacji_zadan.png)
![Ukończenie zadań przez użytkowników](wykres_ukonczenia_zadan.png)
![Podium aktywności](podium_aktywnosci.png)

## Dane

Wykorzystałem cztery endpointy: `/users`, `/posts`, `/comments` i `/todos`.
[Tu 1-2 zdania, dlaczego akurat te: powiązania przez userId i postId, różne rodzaje analiz.]
Teksty postów i komentarzy to Lorem ipsum, więc analizuję strukturę i liczby, a nie treść.

## Metryki i wykresy

- liczba użytkowników, postów, komentarzy i zadań oraz ogólny odsetek wykonanych zadań,
- liczba postów i komentarzy na użytkownika,
- odsetek wykonanych zadań według użytkowników,
- wykresy: pierścieniowy (realizacja zadań), słupkowy (ukończenie zadań użytkowników), podium aktywności.

## Najważniejsze wnioski

- Wykonanych jest 45% zadań (90 z 200).
- Odsetek wykonanych zadań różni się między użytkownikami (30%-60%).
- Posty i komentarze są rozłożone równomiernie (10 postów i 50 komentarzy na użytkownika).
- JSONPlaceholder to dane demonstracyjne, więc wyniki odzwierciedlają strukturę danych.

## Technologie

Python, pandas, requests, Plotly, Google Colab (Jupyter Notebook).

## Jak uruchomić

Otwórz notebook przez link „Demo" powyżej i wybierz *Środowisko wykonawcze → Uruchom wszystko*.
Notebook nie wymaga dodatkowej konfiguracji ani kluczy API.

## Jak użyłem AI

[Uzupełnij prawdziwie i konkretnie, patrz uwagi poniżej.]
