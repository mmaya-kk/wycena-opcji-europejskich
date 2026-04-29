**Wycena Opcji Europejskich: Black-Scholes vs Monte Carlo**

Projekt wykonany w ramach kursu: PwC Market Risk Lab

Ten projekt służy do wyceny opcji kupna (Call) oraz sprzedaży (Put) na rynku kapitałowym. Porównuje on klasyczny model matematyczny **Blacka-Scholesa** z podejściem symulacyjnym **Monte Carlo**.

**Kluczowe analizy**
- **Model Blacka-Scholesa:** Analityczne rozwiązanie wyceny opcji przy użyciu dystrybuanty rozkładu normalnego (funkcja błędu `erf`).
- **Symulacja Monte Carlo:** Numeryczne przybliżenie ceny opcji przy założeniu, że cena instrumentu bazowego podąża za **Geometrycznym Ruchem Browna (GBM)**.
- **Analiza Błędów:** Automatyczne wyliczanie błędu absolutnego i względnego między obiema metodami.
- **Wizualizacja Danych:** Przejrzyste zestawienie wyników w tabeli

**Model Matematyczny**
W projekcie wykorzystano następujące zależności:
* **Geometryczny Ruch Browna:** Modelowanie ścieżek cenowych akcji.
* **Dyskontowanie ciągłe:** Sprowadzanie przyszłych wypłat do wartości bieżącej (Present Value).
* **Zbieżność stochastyczna:** Weryfikacja dokładności symulacji wraz ze wzrostem liczby prób $n$.

**Wnioski**

* Modele działają niemal identycznie: Różnica między wzorem matematycznym (Black-Scholes) a symulacją (Monte Carlo) jest mniejsza niż 0,1%.

* Więcej prób = lepszy wynik: W przypadku opcji Put wyraźnie widać, że zwiększenie liczby symulacji z 10 tys. do 50 tys. "wygładziło" wynik (0.4030% -> 0.0313%)

* Losowość to norma: Niewielkie wahania błędu (jak przy opcji Call) to naturalna cecha metody Monte Carlo. Wynikają one z przypadku przy losowaniu liczb.
