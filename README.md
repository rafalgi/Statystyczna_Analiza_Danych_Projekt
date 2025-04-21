# Statystyczna Analiza Danych Projekt

## Autor
Rafał Gibała

## Opis projektu
Ten projekt obejmuje statystyczną analizę danych giełdowych firmy Apple Inc. (AAPL) w okresie od 2010 do 2020 roku. Analiza obejmuje różne testy statystyczne, wizualizacje oraz modele regresji.

## Zbiór danych
Zestaw danych zawiera kompleksowe informacje o dziennych statystykach dotyczących akcji Apple Inc. (AAPL). Dane obejmują takie wskaźniki, jak:
- Data: Dzień handlowy.
- Cena zamknięcia: Cena akcji na koniec dnia handlowego.
- Wolumen obrotu: Całkowita liczba akcji wymienionych w ciągu danego dnia.
- Cena otwarcia: Cena akcji na początku dnia handlowego.
- Najwyższa cena: Maksymalna cena akcji w ciągu dnia handlowego.
- Najniższa cena: Minimalna cena akcji w ciągu dnia handlowego.

## Pliki
- `Projekt Statystyczna Analiza Danych.ipynb`: Główny notebook zawierający kod analizy danych.
- `HistoricalQuotes.csv`: Plik CSV z danymi historycznymi dotyczącymi akcji Apple Inc.

## Analiza
### 1. Wczytanie danych
Dane są wczytywane do DataFrame przy użyciu biblioteki `pandas`.

### 2. Wstępna analiza danych
- Usunięcie spacji z nazw kolumn.
- Konwersja wartości z formatów tekstowych na numeryczne.

### 3. Wyznaczanie podstawowych parametrów statystycznych
- Średnia, mediana, odchylenie standardowe i inne podstawowe statystyki.

### 4. Testy statystyczne
#### Test Shapiro-Wilka
Sprawdza, czy dane pochodzą z rozkładu normalnego.

#### Test Levene’a
Sprawdza homogeniczność wariancji między grupami.

#### Test T-Studenta
Porównanie średnich dwóch okresów.

#### Test Manna-Whitneya
Nieparametryczny test porównujący mediany dwóch okresów.

#### ANOVA
Analiza wariancji dla miesięcy w 2020 roku.

#### Test Kruskala-Wallisa
Nieparametryczny odpowiednik ANOVA, używany gdy dane nie spełniają założeń normalności.

### 5. Analiza regresji
Regresja liniowa: Cena zamknięcia vs Objętość obrotu (Volume).

### 6. Wizualizacje
- Histogramy i wykresy skrzypcowe dla porównania rozkładów cen w różnych latach.
- Wykresy regresji liniowej.

## Wnioski
Dokonano analizy statystycznej i porównania cen akcji Apple Inc. w różnych latach, wskazując na istotne różnice w rozkładach cen.

## Kontakt
Rafał Gibała - rafal13996@gmail.com
