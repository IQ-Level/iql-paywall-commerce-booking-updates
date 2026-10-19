# Historia wersji — IQL Paywall, Commerce & Booking

Kanał wersji wtyczki. Instalacje czytają stąd `latest.json` (przycisk „Sprawdź teraz”
w Ustawieniach). Paczki ZIP dostajesz tam, gdzie kupiłeś wtyczkę.

## 1.4.2 — 2026-10-19

### Licencje i produkty w panelu
- **Usuwanie licencji** z ekranu licencji albo zbiorczo z listy; unieważnianie też zbiorczo.
- **Data końca aktualizacji** wpisywana wprost albo „bez limitu”.
- **Rodzaj licencji** w produkcie: jednorazowa, subskrypcja albo dożywotnia — widać go
  w sklepie i w programie klienta.
- **Usuwanie produktu** z ekranu edycji, razem z plikami. Produktu z licencjami nie da się
  usunąć przez przypadek. Numer wersji wgranego pliku można poprawić.

### Pakiety i pliki
- **Komponenty**: kilka pluginów pod jednym kluczem (np. Optimizer + Monitor), każdy
  z własnymi wersjami. API licencji podaje wersję wskazanego komponentu.
- Znacznik `{{IQL_LICENSE_KEY}}` w pliku „budowanym pod klienta”: plik działa bez
  wpisywania klucza.

### Poprawki
- Kasa i kreator rezerwacji obok Elementora 4 bez podwójnych pozycji.
- Kreator rezerwacji dopasowuje układ do szerokości widżetu.
- Edytor grafiku tygodnia w panelu znów pokazuje dni.

Wgraj `iql-paywall-commerce-booking-1.4.2.zip` jak poprzednio, potem wyczyść cache strony.

## 1.4.1 — 2026-10-18

- **Licencja wtyczki prościej:** klucz publiczny jest wbudowany, wystarczy wkleić klucz IQLB.
- **Poprawka:** w motywach klasycznych formularz zakupu pokazywał ten sam produkt dwa razy
  (skrypty ładowały się podwójnie). Dotyczyło też kreatora rezerwacji i konta klienta.
- **Poprawka:** na ekranie produktu ramka „Gdzie oferować” wchodziła pod pole nazwy.
- Formularz zakupu wyjaśnia, że domenę licencji podaje się dopiero przy aktywacji.

Wgraj `iql-paywall-commerce-booking-1.4.1.zip` jak poprzednio, potem wyczyść cache strony
(np. W3 Total Cache), żeby goście dostali nowy HTML.

## 1.4.0 — 2026-10-18

### Uporządkowany panel
- Menu ma krótką nazwę i sekcje **Sprzedaż** (Zamówienia, Produkty, Licencje)
  i **Rezerwacje** (Wizyty, Usługi, Specjaliści). Płatności, Wygląd, E-maile
  i Licencja wtyczki są zakładkami **Ustawień**, Grafiki — zakładką Specjalistów.
  Stare adresy stron działają.
- **Moduły** do wyłączenia (Ustawienia → Ogólne): Rezerwacje, Sprzedaż, Licencje
  i pliki. Domyślnie wszystko działa jak dotąd.

### Sklep
- Nowy ekran produktu jak w WooCommerce: edytor opisu, obrazek i galeria,
  zakładki „Dane produktu”, cechy „Do pobrania” i „Licencja”.
- Na stronę: karta produktu `[iqlb_product]`, siatka `[iqlb_products]`, konto klienta
  `[iqlb_account]` — także jako widgety Elementora.
- Produkty cyfrowe: pliki w wersjach poza biblioteką mediów, podpisane linki do
  pobrania, znak wodny pod klienta. Licencje z domenami, okresem aktualizacji
  i przedłużeniem, API licencji dla programu klienta.
- Kasa: VAT (domyślnie wyłączony) z odwrotnym obciążeniem dla firm z UE, dane do
  faktury, zgoda na natychmiastowe dostarczenie treści cyfrowej, produkty za 0 zł.
- Przelewy24 (BLIK, przelewy, karty). Stripe może pokazywać metody z jego panelu.

### Poprawka
- Formularze panelu zapisywały cudzysłowy z ukośnikiem (nazwa produktu, edytowany
  szablon maila).

### Aktualizacja
Wgraj `iql-paywall-commerce-booking-1.4.0.zip` przez **Wtyczki → Dodaj nową → Wyślij
wtyczkę** i nadpisz obecną wersję. Dane zostają, baza uzupełnia się sama.

## 1.3.0 — 2026-09-16

- Panel informuje o nowej wersji wtyczki (Ustawienia + pasek na liście wtyczek).
- Zmiana nazwy na **IQL Paywall, Commerce & Booking**. WordPress widzi ją jako osobną
  wtyczkę: aktywuj nową, dezaktywuj i usuń starą „IQL Paywall & Booking”. Dane zostają.
