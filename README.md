# gdzie-mieszkac-lodz-data

Dane (generowane, nie edytować ręcznie) dla strony „Gdzie mieszkać w Łodzi?"
(`gisboost.github.io/mapy-analizy/gdzie-mieszkac-lodz/`; kod w repo [mapy-analizy](https://github.com/GISBoost/mapy-analizy)).

Zawartość: `manifest.json` (wersje metody, okna, krzywe), `hex.json` (siatka hex 250 m), `layers.json` (warstwy
statyczne i hałas per heks), `m/*.bin` (macierze czasów O–D, odczyt przez HTTP `Range`). Format i metoda:
[easy-R5/tools/apartment_finder](https://github.com/GISBoost/easy-R5/tree/main/tools/apartment_finder).

**Historia git jest celowo jednokomitowa** (gałąź `gh-pages`, nadpisywana `--force` przez
`scripts/publish_data.sh` z easy-R5): dane to ok. 250 MB binariów przy każdej regeneracji, a historia urosłaby
ponad limit repozytorium. Nie opieraj się na starszych commitach.

Źródła: OpenStreetMap (ODbL), GTFS ZDiT Łódź i zrekonstruowany GTFS-RT (`GISBoost/easy-GTFS-RT`), ŁKA, mapa
akustyczna Łodzi (Urząd Miasta Łodzi, informacja publiczna; według autora projektu można ją pobierać, modyfikować
i rozpowszechniać; brak odrębnej licencji na stronie źródła).
