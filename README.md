# receptury.dysza.app — Receptury

Moduł Dysza.App dla Pracowni Sushi (DYSZA 2.0): droga produktu od towaru z FIRMINO do klienta —
towar → surowiec (przelicznik i wydajność) → półprodukt (partia i ile z niej wychodzi) → produkt (gramatury na 1 szt.)
→ zestaw (sklep i tablet) → paczka (z opakowaniami, dowóz i odbiór) albo talerz (stolik).

Każdy zapis receptury to nowa wersja od jutra; zużycie za minione dni liczy się według wersji, która wtedy obowiązywała.
Wersję zaplanowaną można jeszcze poprawić albo wycofać. Koszt liczy się z cen zakupu (netto) z eksportu „Produkty”
z FIRMINO, który wgrywa Dyrektor Produkcji; zużycie nominalne — ze sprzedaży zestawów w DYSZY z ostatnich 30 dni.
Alergeny surowców to najpierw propozycje z nazw towarów — po sprawdzeniu z etykietą Dyrektor Produkcji je potwierdza.

Wchodzą osoby z dostępem do modułu „receptury” w manager.dysza.app i Architekt. Strona nie zawiera danych ani imion
i adresów osób; wszystko przychodzi z funkcji bazy `receptury_*` i `firmino_towary_wgraj`, które same pilnują dostępu.

Jeden plik `index.html`: ten sam szablon i ta sama logika co w pokazie modułu, mały silnik szablonu bez bibliotek,
logowanie przez wspólne okno dysza.app (login z karty i PIN z managera).

Półprodukt liczymy w g, ml albo szt. (np. wywar w ml). Niebieskie „i” obok kafelka z imieniem otwiera aktualną instrukcję (PDF)
ze stałego linku na Dysku Google — nową wersję podmienia tam automat ZDZISŁAW Instrukcje.

Wersja 1.2 · 2026-11-18 17:01 · 226d633
