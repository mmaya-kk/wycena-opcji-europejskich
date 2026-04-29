# wycena-opcji-europejskich
Projekt wykonany w ramach kursu: PwC Market Risk Lab
# Wycena Opcji Europejskich: Black-Scholes vs Monte Carlo

Ten projekt służy do wyceny opcji kupna (Call) oraz sprzedaży (Put) na rynku kapitałowym. Porównuje on klasyczny model matematyczny **Blacka-Scholesa** z podejściem symulacyjnym **Monte Carlo**.

## 🚀 Główne Funkcjonalności
- **Model Blacka-Scholesa:** Analityczne rozwiązanie wyceny opcji przy użyciu dystrybuanty rozkładu normalnego (funkcja błędu `erf`).
- **Symulacja Monte Carlo:** Numeryczne przybliżenie ceny opcji przy założeniu, że cena instrumentu bazowego podąża za **Geometrycznym Ruchem Browna (GBM)**.
- **Analiza Błędów:** Automatyczne wyliczanie błędu absolutnego i względnego między obiema metodami.
- **Wizualizacja Danych:** Przejrzyste zestawienie wyników w formie tabelarycznej przy użyciu biblioteki `pandas`.

## 📈 Model Matematyczny
W projekcie wykorzystano następujące zależności:
* **Geometryczny Ruch Browna:** Modelowanie ścieżek cenowych akcji.
* **Dyskontowanie ciągłe:** Sprowadzanie przyszłych wypłat do wartości bieżącej (Present Value).
* **Zbieżność stochastyczna:** Weryfikacja dokładności symulacji wraz ze wzrostem liczby prób $n$.
