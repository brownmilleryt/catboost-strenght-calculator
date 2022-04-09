# catboost-strenght-calculator

Beton jest najważniejszym materiałem w inżynierii lądowej i wodnej. Wytrzymałość betonu na ściskanie jest wysoce nieliniową funkcją wieku i składników. Składniki te obejmują cement, żużel wielkopiecowy, popiół lotny, wodę, superplastyfikator, kruszywo grube i kruszywo drobne.

Rzeczywista wytrzymałość betonu na ściskanie (MPa) dla danej mieszanki w określonym wieku (dni) została określona w laboratorium. Dane są w postaci surowej (nieskalowanej). Dane zawierają 8 ilościowych zmiennych wejściowych i 1 ilościową zmienną wyjściową (Wytrzymałość na ściskanie) oraz 1030 przypadków (obserwacji).

Ponieważ jest to problem regresji, do oceny modelu użyjemy błędu średniokwadratowego (Root mean square error)

Jest to modyfikacja moich wcześniejszych modeli. 

Wyjściowy plik w formacie .xlsx będzie zawierał zarówno predykcję wytrzymałości na ściskanie po 28 dniach jak i ocenę przyrostu wytrzymałości w czasie (do 28 dni) oraz porównanie tabelaryczne modeli. 

W niniejszym opracowaniu zostaną wykorzystane następujące modele:
1. Model regresji grzbietowej (ridge regression)
2. Model regresji LASSO (least absolute shrinkage and selection operator)
3. Model regresji sieci elastycznej (elastic net)
4. Model regresji opartej na sekwencja drzew regresji (decision tree regression)
5. cnd....




## Cel projektu

Celem projektu jest opracowanie uproszczonego modelu predykcji wytrzymałości betonu na ściskanie na który będą mogli wykorzystywać studenci kierunków budownictwo i inżynieria materiałowa a w przyszłości aplikację która do trenowania modeli będzie przyjmować wartości wprowadzone do arkusza kalkulacjnego
