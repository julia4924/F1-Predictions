# Predykcja DNF w wyścigach Formuły 1 z użyciem uczenia maszynowego

Celem projektu jest przewidywanie, czy kierowca Formuły 1 **nie ukończy wyścigu** (DNF – *Did Not Finish*), na podstawie danych wyścigowych, pogodowych i technicznych. W projekcie zastosowano klasyfikację binarną z wykorzystaniem technik takich jak regresja logistyczna, las losowy oraz XGBoost.

## Kluczowe elementy projektu

- **Zmienna docelowa**: `DNF` (0 – ukończył wyścig, 1 – nie ukończył)
- **Analiza danych**: korelacje, rozkłady, klastrowanie (pogoda, styl jazdy)
- **Modelowanie**: regresja logistyczna, random forest, XGBOOST,KNN,SVM
- **Strojenie hiperparametrów**: `tune_grid`, `tune_bayes`
- **Ewaluacja modeli**: accuracy, ROC AUC, confusion matrix, wykresy ROC
- **Najlepszy model**: XGBoost Undersampled (AUC ≈ 0.98)


## Wnioski

Analiza potwierdziła, że czynniki takie jak agresja kierowcy, strategia pit-stopów oraz warunki pogodowe znacząco wpływają na ryzyko nieukończenia wyścigu. Model XGBoost Undersampled osiągnął najwyższą skuteczność i może być z powodzeniem zastosowany w analizach predykcyjnych F1.



