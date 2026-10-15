# Analiza danych z API JSONPlaceholder

Projekt pobiera dane z publicznego API JSONPlaceholder, oblicza podstawowe statystyki
i przedstawia wyniki na wykresach. Powstał jako zadanie rekrutacyjne.

**Demo:** [Otwórz notebook w Google Colab](https://colab.research.google.com/github/Wozniak-Kacper/analiza-danych-api/blob/main/analizaAPI.ipynb)

## Zrzuty ekranu

![Podsumowanie realizacji zadań](podsumowanie_realizacji_zadan.png)
![Ukończenie zadań przez użytkowników](wykres_ukonczenia_zadan.png)
![Podium aktywności](podium_aktywnosci.png)

## Dane

Wykorzystałem cztery endpointy: /users, /posts, /comments i /todos. Ich wybór pozwala połączyć dane o użytkownikach z ich postami, komentarzami i zadaniami, wykorzystując identyfikatory userId oraz postId. Dzięki temu mogłem przeanalizować aktywność użytkowników, liczbę komentarzy oraz stopień realizacji zadań. Teksty postów i komentarzy mają charakter demonstracyjny, dlatego analiza koncentruje się na strukturze danych i wartościach liczbowych, a nie na treści tekstowej.

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

Otwórz notebook przez link „Demo” powyżej. Bez logowania do Google możesz przeglądać kod, opisy i zapisane wyniki. Aby uruchomić komórki i ponownie wykonać analizę, musisz zalogować się na konto Google.
Po zalogowaniu wybierz Środowisko wykonawcze → Uruchom wszystko. Notebook nie wymaga dodatkowej konfiguracji ani kluczy API.

## Proces pracy i użycie AI

To mój pierwszy projekt, w którym samodzielnie pobieram i analizuję dane z zewnętrznego API.
Pythona poznałem wcześniej na uczelni przy uczeniu maszynowym, a Google Colab poznałem na
kolejnym przedmiocie, na którym też będę używał Pythona. Dlatego wybrałem właśnie to środowisko.
Rozważałem też prezentację wyników w Streamlit, ale nie da się go uruchomić bezpośrednio w Colabie,
więc zostałem przy notebooku.

**Jak korzystałem z AI:**

- **Plan projektu:** z pomocą AI (Claude) ustaliłem kolejne etapy pracy. Po przeanalizowaniu
  planu wprowadziłem własne korekty, zostawiając to, co uznałem za wartościowe, i odrzucając elementy zbędne.
- **Wybór danych:** strukturę danych sprawdziłem na stronie JSONPlaceholder i na jej podstawie
  wybrałem endpointy do analizy.
- **Kod:** generowałem go z pomocą AI (ChatGPT) fragmentami, krok po kroku. Każdy fragment
  analizowałem, wprowadzałem poprawki i starałem się zrozumieć, co robi. Część linii pisałem
  samodzielnie, żeby lepiej nauczyć się biblioteki np. pobranie kolejnych endpointów.
- **Metryki:** w kolejnych etapach sam decydowałem, jakie metryki policzyć (wybrałem te, które
  wydały mi się najciekawsze), i formułowałem odpowiednie prompty.
- **Opisy w notebooku i wnioski:** powstały z pomocą AI (ChatGPT), a następnie je
  sprawdziłem i dostosowałem.
