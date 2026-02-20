# CLAUDE.md — Instrukcja dla Claude

## Czym jest to repozytorium?

Publiczny roadmap nauki do zawodu **AI/Agent Engineera**. Autor (Łukasz) zaczyna od podstaw i dokumentuje swoją drogę. Repozytorium służy dwóm celom: jako jego własny dziennik nauki i jako materiał, który może przydać się innym w podobnej sytuacji.

Treść jest w **języku polskim**. Zawsze pisz po polsku.

---

## Dla kogo są te materiały?

Dla osoby, która **nie ma pojęcia o AI**. Zna podstawy programowania i matematyki na poziomie liceum, ale terminy takie jak "sieć neuronowa", "model", "klasyfikator", "loss function" są dla niej obce.

Kiedy w lekcji pojawia się pojęcie AI — zawsze krótko wytłumacz co to jest, zanim go użyjesz. Nie zakładaj żadnej wiedzy o AI.

---

## Struktura repozytorium

```
roadmap/
  step 0 - Przygotowanie/
    README.md               ← lista wszystkich tematów do opanowania
    lesson 1 - Matematyka/
      matematyka.md         ← przegląd lekcji z linkami
      1. Podstawy algebry liniowej (wektory, macierze).md
      2. Funkcje i wykresy.md
      3. Pochodne i całki (...).md
      ... kolejne lekcje
    lesson 2 - Python/
    lesson 3 - Generative AI/
    lesson 4 - SQL/
    lesson 5 - Machine Learning/
    lesson 6 - Narzędzia i Środowisko/
    lesson 7 - Dodatkowe Zagadnienia/
  step 1 - ...  (przyszłe kroki)
```

Każdy "step" to etap nauki. Każdy "lesson" to osobna dziedzina. W każdym lesson jest plik przeglądowy (np. `matematyka.md`) z checklistą tematów i linkami do poszczególnych plików z lekcjami.

---

## Jak pisać lekcje — zasady stylu

### Zasada nadrzędna

**Najpierw intuicja i opis, potem wzór.** Wzory i formalne definicje pojawiają się jako wsparcie dla zrozumiałego tekstu — nie zamiast niego.

### Struktura każdej sekcji w pliku

Każdy temat w lekcji (oznaczony nagłówkiem `## N. Tytuł`) ma następujący układ:

1. **Otwierasz analogią lub historyjką z życia** — coś, co czytelnik już zna. "Wyobraź sobie...", "Pomyśl o...", "Kiedy...", itp.
2. **Tłumaczysz pojęcie w plain language** — zanim pokażesz wzór.
3. **Wzory i obliczenia jako ilustracja** — w blokach kodu, z komentarzami wyjaśniającymi każdy krok.
4. **Kończysz krótką wzmianką o AI** w formacie:

```
> **W AI:** Jedno do trzech zdań. Wyjaśnij jak ten temat matematyczny łączy się z AI.
> Zakładaj zero wiedzy o AI — jeśli używasz terminu (np. "model"), wyjaśnij go jednym zdaniem.
```

### Jak wygląda zatwierdzony styl w praktyce

Przykład dobrego otwarcia sekcji (z lekcji o funkcjach):

> Wyobraź sobie automat z kawą. Wciskasz przycisk "espresso" i dostajesz espresso. Wciskasz "latte" i dostajesz latte. Kluczowe jest to, że jeden przycisk daje zawsze **dokładnie jeden** określony napój — nigdy nie zdarza się, że wciskasz espresso i raz wychodzi kawa, a raz zupa.
>
> Właśnie tak działa funkcja w matematyce. **Funkcja to reguła, która każdej wartości wejściowej przypisuje dokładnie jedną wartość wyjściową.**

Wzór pojawia się *po* tym wyjaśnieniu, jako formalne zapisanie tego co już rozumiemy.

### Co NIE działa — błędy z poprzednich iteracji

❌ **Nie dziel pliku na "CZĘŚĆ I: Matematyka" i "CZĘŚĆ II: Jak to działa w AI?"** — taki podział sprawia że lekcja wygląda jak dwa osobne dokumenty i AI trafia na sam koniec, oderwane od kontekstu.

❌ **Nie otwieraj lekcji tabelką "Gdzie w AI / Co tam robi..."** — to zakłada wiedzę o AI której czytelnik nie ma.

❌ **Nie pisz ścianą wzorów** — blok `f'(x) = lim_{h→0} [f(x+h)-f(x)]/h` bez wyjaśnienia co to znaczy i po co to liczymy jest bezużyteczny.

❌ **Nie używaj terminów AI bez wyjaśnienia** — słowa takie jak "trening modelu", "backpropagation", "loss function", "embedding" muszą być wyjaśnione gdy się pojawiają. Czytelnik ich nie zna.

❌ **Nie bądź zwięzły kosztem zrozumienia** — lepiej trzy zdania tłumaczące niż jedno zdanie techniczne.

---

## Format pliku z lekcją

```markdown
# 📌 Tytuł Lekcji

---

## 1. Pierwszy temat

[Akapit z analogią / historyjką otwierającą]

[Wytłumaczenie pojęcia w plain language]

[Blok kodu z przykładami, obliczeniami, diagramami ASCII]

> **W AI:** Krótka wzmianka jak to się używa w AI, dla totalnego żółtodzioba.

---

## 2. Drugi temat

...

---

## ✅ Sprawdź się

1. Pytanie...
2. Pytanie...

<details>
<summary>Odpowiedzi</summary>

1. Odpowiedź...
2. Odpowiedź...

</details>
```

### Szczegóły techniczne

- Emoji w tytule pliku (`# 📈 Funkcje i Wykresy`) — tak
- Numerowane nagłówki sekcji (`## 1. Czym jest funkcja?`) — tak
- Emoji w nagłówkach sekcji (`## 1️⃣ WEKTORY`) — **nie**, to stary styl
- Diagramy ASCII dla wykresów i wizualizacji — tak, bardzo pomocne
- Bloki kodu (` ``` `) do przykładów numerycznych i obliczeń krok po kroku — tak
- Pogrubienie (`**tekst**`) dla kluczowych definicji — tak, ale z umiarem
- Quiz "Sprawdź się" na końcu z odpowiedziami ukrytymi w `<details>` — tak

---

## Nazewnictwo plików

Pliki z lekcjami w folderze `lesson X - Nazwa/`:

```
N. Tytuł lekcji.md

np.:
1. Podstawy algebry liniowej (wektory, macierze).md
2. Funkcje i wykresy.md
3. Pochodne i całki (podstawy rachunku różniczkowego).md
```

Liczba na początku określa kolejność w checkliście z `README.md` danego step.

Plik przeglądowy (np. `matematyka.md`) zawiera:
- Krótki wstęp czym jest ta dziedzina
- Checklistę tematów z linkami do poszczególnych plików lekcji

---

## Ton i głos

- Bezpośredni, ale przyjazny — "wyobraź sobie", "pomyśl o tym jak o...", "nie przejmuj się na razie..."
- Nie akademicki, nie formalny
- Motywujący tam gdzie trzeba — wyjaśniaj PO CO dany temat jest ważny, ale przez konkretny przykład, nie przez abstrakcyjne zapewnienia
- Kiedy temat jest trudny — powiedz to wprost i obiecaj że to normalne

---

## Git

Branch do pracy: `claude/add-math-lessons-tB8zC` (lub nowy branch dla nowych funkcjonalności — zawsze zaczynający się od `claude/`).

Commity po polsku lub angielsku, opisowe.
