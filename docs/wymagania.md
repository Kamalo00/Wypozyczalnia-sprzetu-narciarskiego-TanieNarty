# **Wypożyczalnia sprzętu narciarskiego – wymagania**

### **1.Wymagania funkcjonalne**

MoSCoW: **M** \= Must, **S** \= Should, **C** \= Could, **W** \= Won't 

| ID | User story | Kryteria akceptacji | MoSCoW |
| :---- | :---- | :---- | :---- |
| 1 | Jako klient chcę zobaczyć sprzęt dostępny w wybranym terminie, aby wiedzieć, co mogę wypożyczyć. | Po podaniu dat i typu sprzętu lista zawiera tylko egzemplarze wolne w całym okresie; widoczna jest cena za okres. | M |
| 2 | Jako klient chcę zarezerwować sprzęt | Rezerwacja blokuje wybrane egzemplarze | M |
| 3 | Jako klient chcę anulować rezerwację, gdy zmienią się moje plany. | Anulowanie zwalnia egzemplarze od razu; nie można anulować rezerwacji już wydanej. | S |
| 4 | Jako sprzedawca chcę wydać sprzęt na podstawie rezerwacji | Rezerwację znajduję po numerze lub nazwisku; po wydaniu status zmienia się na „Wypożyczone”. | M |
| 5 | Jako sprzedawca chcę przyjąć zwrot i ocenić stan sprzętu, aby zamknąć wypożyczenie. | Zwrot bez uwag zwalnia sprzęt; przy uszkodzeniu zapisuję opis i koszt, a sprzęt oznaczam jako niedostępny. | M |
| 6 | Jako sprzedawca chcę zarządzać katalogiem sprzętu i cennikiem, aby oferta była aktualna. | Mogę dodać, edytować i wycofać sprzęt oraz ustawić cenę za dobę | M |
| 7 | Jako sprzedawca chcę zarejestrować wypożyczenie bez rezerwacji, aby obsłużyć klienta, który przyszedł na miejscu. | System pokazuje tylko wolne egzemplarze; wypożyczenie wymaga danych klienta. | S |
| 8 | Jako sprzedawca chcę, aby system sam liczył opłatę i karę za spóźnienie, aby uniknąć pomyłek. | Opłata \= liczba dób × cena; za każdą rozpoczętą dobę spóźnienia dolicza się karę z cennika. | M |
| 9 | Jako sprzedawca chcę, aby system wygaszał rezerwacje, po które nikt nie przyszedł | Rezerwacja nieodebrana do końca pierwszego dnia zmienia status na „Wygasła” i zwalnia sprzęt. | S |
| 10 | Jako sprzedawca chcę prosty raport przychodów za okres. | Raport pokazuje sumę opłat za wybrany okres; eksport do CSV. | C |
| 11 | Jako klient chcę dostać potwierdzenie rezerwacji e-mailem. | E-mail z numerem i terminem wysyłany po utworzeniu rezerwacji. | C |
| 12 | Jako klient chcę mieć dostęp do różnych form płatności, poprzez aplikacje | Poza zakresem tej wersji. Opłata jest pobierana na miejscu | W |

### **2 Wymagania niefunkcjonalne**

| ID | Kategoria | Wymaganie |
| :---- | :---- | :---- |
| 1 | Poprawność danych | Niemożliwa podwójna rezerwacja tego samego egzemplarza (kontrola nakładania terminów w transakcji). |
| 2 | Wydajność | Wyszukiwanie dostępnego sprzętu trwa poniżej 2 s dla katalogu do 1000 egzemplarzy. |
| 3 | Bezpieczeństwo | Logowanie sprzedawcy, hasła przechowywane jako skróty, dostęp do panelu sprzedawcy tylko po zalogowaniu. |
| 4 | Ochrona danych | Przechowujemy tylko imię, nazwisko i kontakt klienta (RODO). |
| 5 | Użyteczność | Wydanie sprzętu zajmuje sprzedawcy maksymalnie 5 kliknięć od znalezienia rezerwacji. |


