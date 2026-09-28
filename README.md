# Wyjaśnialna Sztuczna Inteligencja (XAI) w Systemach Wspomagania Decyzji – Praca Magisterska

Repozytorium zawiera kod źródłowy, skrypty do przetwarzania danych oraz wyniki analiz zrealizowanych na potrzeby mojej pracy magisterskiej na kierunku Analityka Gospodarcza. Projekt skupia się na zastosowaniu i ewaluacji technik Explainable AI (SHAP, LIME) w celu zwiększenia transparentności i interpretowalności modeli uczenia maszynowego (uczenie nadzorowane).

## Cel Projektu
Głównym celem badawczym było zbadanie, w jaki sposób metody XAI mogą wspierać procesy decyzyjne w biznesie poprzez wyjaśnianie predykcji złożonych modeli (tzw. "czarnych skrzynek", np. XGBoost) w porównaniu do tradycyjnych, wysoce interpretowalnych algorytmów, takich jak regresja logistyczna. Analiza została przeprowadzona na zróżnicowanych problemach klasyfikacyjnych.

## Wykorzystane Zbiory Danych
W ramach analizy porównawczej przetestowano modele na trzech uniwersalnych zbiorach danych, reprezentujących różne domeny biznesowe:
* **Default of Credit Card Clients (Ryzyko Kredytowe):** Przewidywanie niewypłacalności klientów (Credit Scoring / Gini index).
* **Telco Customer Churn (Telekomunikacja):** Identyfikacja czynników wpływających na rezygnację klientów z usług.
* **IBM HR Analytics Employee Attrition (Zasoby Ludzkie):** Analiza prawdopodobieństwa odejścia pracowników z firmy.

## Technologie i Metodologia
* **Język:** Python (oraz skrypty w R)
* **Modele predykcyjne:** XGBoost, Regresja Logistyczna (Logistic Regression)
* **Techniki XAI:** SHAP (SHapley Additive exPlanations), LIME (Local Interpretable Model-agnostic Explanations)
* **Ewaluacja i przetwarzanie:** `scikit-learn`, `pandas`, `numpy`, wyliczanie współczynnika Giniego oraz metryk AUC-ROC.
* **Eksploracyjna Analiza Danych (EDA):** `seaborn`, `matplotlib`, analiza multikolinearności (VIF).

## Zawartość Repozytorium
* **`EDA/`** – Skrypty do kompleksowej analizy eksploracyjnej, wizualizacji rozkładów zmiennych, statystyk opisowych oraz korelacji.
* **`Preprocessing/`** – Kod odpowiedzialny za czyszczenie danych, transformacje, Label Encoding oraz One-Hot Encoding dla zmiennych kategorialnych.
* **`Models/`** – Implementacja modeli predykcyjnych, strojenie hiperparametrów i ocena jakości (Gini, ROC AUC).
* **`XAI_Analysis/`** – Generowanie lokalnych i globalnych wyjaśnień modeli za pomocą bibliotek SHAP i LIME, wizualizacje wpływu poszczególnych cech na decyzje modelu.

---
*Autor:* Aleksandra Jaworska
