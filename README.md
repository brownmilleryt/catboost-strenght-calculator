# catboost-strenght-calculator

Beton jest najważniejszym materiałem w inżynierii lądowej i wodnej. Wytrzymałość betonu na ściskanie jest wysoce nieliniową funkcją wieku i składników. Składniki te obejmują cement, żużel wielkopiecowy, popiół lotny, wodę, superplastyfikator, kruszywo grube i kruszywo drobne.

Rzeczywista wytrzymałość betonu na ściskanie (MPa) dla danej mieszanki w określonym wieku (dni) została określona w laboratorium. Dane są w postaci surowej (nieskalowanej). Dane zawierają 8 ilościowych zmiennych wejściowych i 1 ilościową zmienną wyjściową (Wytrzymałość na ściskanie) oraz ponad 1000 przypadków (obserwacji).

Recepty miesanki betonowej były oparte w większości na cementach CEM I (R) CEM II/A (R) a zbiór danych został opracowany podczas zarobów próbnych na WBT.

Ponieważ jest to problem regresji, do oceny modelu użyjemy błędu średniokwadratowego (Root mean square error)

Jest to modyfikacja moich wcześniejszych modeli. 

### Wyjściowy plik w formacie .xlsx będzie zawierał zarówno predykcję wytrzymałości na ściskanie po 28 dniach, ocenę przyrostu wytrzymałości w czasie (do 28 dni) oraz porównanie tabelaryczne różnych modeli wykorzystywanych w uczeniu maszynowym. 

### Wyjściowy plik w formacie .xlsx będzie plikiem modyfikowalnym a cały skrypt zapisany w formacie edytowalnego notatnika Jupyter dzięki czemu będzie możliwa bieżąca zmiana składników w mieszance betonowej i śledzenie ich wpływu na przewidywaną wytrzymałość betonu.

W niniejszym opracowaniu zostaną wykorzystane następujące modele:
1. Model regresji grzbietowej (ridge regression)
2. Model regresji LASSO (least absolute shrinkage and selection operator)
3. Model regresji sieci elastycznej (elastic net)
4. Model regresji opartej na sekwencja drzew regresji (decision tree regression)
5. cnd....




## Cel projektu

Celem projektu jest opracowanie uproszczonego modelu predykcji wytrzymałości betonu na ściskanie na który będą mogli wykorzystywać studenci kierunków budownictwo i inżynieria materiałowa a w przyszłości aplikację która do trenowania modeli będzie przyjmować wartości wprowadzone do arkusza kalkulacjnego.

## Zastosowanie

Używając niniejszego modelu możliwe będzie zbudowanie modeli uczenia maszynowego do przewidiwyania wytrzymałości betonu na ściskanie na podstawie takich parametrów jak zawartość powietrza, temperatura w okresie dojrzewania etc. 
