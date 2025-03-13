# Projekt Statystyczna Analiza Danych

## Autor
Rafał Gibała

## Zbiór danych
Ten zestaw danych zawiera kompleksowe informacje o dziennych statystykach dotyczących akcji Apple Inc. (AAPL) w okresie od 2010 do 2020 roku. Dane obejmują takie wskaźniki, jak cena zamknięcia, wolumen obrotu, cena otwarcia, najwyższa cena i najniższa cena.

Zbiór danych zawiera następujące kolumny:
- **Data:** Dzień handlowy.
- **Cena zamknięcia:** Cena akcji na koniec dnia handlowego.
- **Wolumen obrotu:** Całkowita liczba akcji wymienionych w ciągu danego dnia.
- **Cena otwarcia:** Cena akcji na początku dnia handlowego.
- **Najwyższa cena:** Maksymalna cena akcji w ciągu dnia handlowego.
- **Najniższa cena:** Minimalna cena akcji w ciągu dnia handlowego.

## Wczytanie danych
```python
import pandas as pd
import numpy as np
from scipy.stats import ttest_ind, shapiro, mannwhitneyu, f_oneway
from sklearn.linear_model import LinearRegression
import matplotlib.pyplot as plt
import seaborn as sns
import scipy.stats as stats
from sklearn.metrics import r2_score

import warnings
warnings.filterwarnings("ignore")

# Wczytanie danych do DataFrame
file_path = 'HistoricalQuotes.csv'
data = pd.read_csv(file_path)
data
