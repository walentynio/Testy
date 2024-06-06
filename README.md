# Testy

==============================================================================================================================================================================================================================================================================================================
================================================================================
I-2_00_PA	PA/PR z towarami we wszystkich stawkach PTU
I-2_00_PR
================================================================================
Zaprogramowac w badanej kasie nastepujace stawki PTU:
A	23%
B	8%
C	3%
D	ZW
E	0%
F	1%
G	2%
W kasie autonomicznej zaprogramowac 7 towarów ("Towar-A".. "Towar-G") w kazdej ze stawek z ceną 1 PLN.
Wystawic PA/PR na 7 towarow o kolejnych nazwach okreslonych powyzej, kazdy towar w innej stawce z iloscia 1,00 i z cena 1 PLN. 
Platnosc gotowka w kwocie 7 PLN.

Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).

1.Zaprogramowac w badanej kasie nastepujace stawki PTU:
```
{ "commandInput": { "A": { "type": 0, "value": 23 }, "B": { "type": 0, "value": 8 }, "C": { "type": 0, "value": 3 }, "D": { "type": 1, "value": 0 }, "E": { "type": 0, "value": 0 }, "F": { "type": 0, "value": 1 }, "G": { "type": 0, "value": 2 } }, "commandType": 3 }
```
2.W kasie autonomicznej zaprogramowac 7 towarów ("Towar-A".. "Towar-G") w kazdej ze stawek z ceną 1 PLN.
Wystawic PA/PR na 7 towarow o kolejnych nazwach okreslonych powyzej, kazdy towar w innej stawce z iloscia 1,00 i z cena 1 PLN. 
Platnosc gotowka w kwocie 7 PLN.

Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).

```
{ "commandType": 30, "commandInput": { "1": { "commandType": 16 }, "2": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-B", "price": 1, "ptu": "B", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "4": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-C", "price": 1, "ptu": "C", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "5": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-D", "price": 1, "ptu": "D", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "6": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-E", "price": 1, "ptu": "E", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "7": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-F", "price": 1, "ptu": "F", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "8": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-G", "price": 1, "ptu": "G", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "9": { "commandType": 24, "commandInput": { "name": "paymentName", "payment_type": 1, "value": 7, "payment_without_terminal": true } }, "10": { "commandType": 26, "commandInput": { "canceled": false }, "print": true, "returnPDF": false, "returnQR": true } } }
```
3. polecenie dla PA
 ```
{ "commandType": 30, "commandInput": { "1": { "commandType": 16 }, "2": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-B", "price": 1, "ptu": "B", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "4": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-C", "price": 1, "ptu": "C", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "5": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-D", "price": 1, "ptu": "D", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "6": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-E", "price": 1, "ptu": "E", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "7": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-F", "price": 1, "ptu": "F", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "8": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-G", "price": 1, "ptu": "G", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "9": { "commandType": 24, "commandInput": { "name": "paymentName", "payment_type": 1, "value": 7, "payment_without_terminal": true } }, "10": { "commandType": 26, "commandInput": { "canceled": true }, "print": true, "returnPDF": false, "returnQR": true } } }
```  

==============================================================================================================================================================================================================================================================================================================
================================================================================
I-2_01_PA	PA/PR z towarami w standardowych stawkach PTU
I-2_01_PR
================================================================================
Zaprogramować w badanej kasie następujące stawki PTU ("-" oznacza stawkę niezaprogramowaną):
A	23%
B	8%
C	3%
D	ZW
E	-
F	-
G	-
Nie zmieniac tak zaprogramowanych stawek PTU do końca testu I-2.
Wystawic PA/PR na 4 towary, kazdy towar w innej stawce z iloscia 1,00 i z ceną 1 PLN. 
Platnosc gotowka w kwocie 4 PLN.
Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).

1. Zaprogramować w badanej kasie następujące stawki PTU ("-" oznacza stawkę niezaprogramowaną):
```
{ "commandInput": { "A": { "type": 0, "value": 23 }, "B": { "type": 0, "value": 8 }, "C": { "type": 0, "value": 3 }, "D": { "type": 1, "value": 0 }, "E": { "type": 2, "value": 0 }, "F": { "type": 2, "value": 0 }, "G": { "type": 2, "value": 0 } }, "commandType": 3 }
```
2. Wystawic PA/PR na 4 towary, kazdy towar w innej stawce z iloscia 1,00 i z ceną 1 PLN. 
```
{ "commandType": 30, "commandInput": { "1": {"commandType": 16}, "2": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-B", "price": 1, "ptu": "B", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "4": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-C", "price": 1, "ptu": "C", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "5": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-D", "price": 1, "ptu": "D", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "6": { "commandType": 24, "commandInput": { "name": "paymentName", "payment_type": 1, "value": 4, "payment_without_terminal": true } }, "7": { "commandType": 26, "commandInput": {"canceled": false}, "print": true, "returnPDF": false, "returnQR": true } } }
```
3. polecenie dla PA
```
{ "commandType": 30, "commandInput": { "1": {"commandType": 16}, "2": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-B", "price": 1, "ptu": "B", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "4": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-C", "price": 1, "ptu": "C", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "5": { "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-D", "price": 1, "ptu": "D", "unit": "" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }, "6": { "commandType": 24, "commandInput": { "name": "paymentName", "payment_type": 1, "value": 4, "payment_without_terminal": true } }, "7": { "commandType": 26, "commandInput": {"canceled": true}, "print": true, "returnPDF": false, "returnQR": true } } }
```
==============================================================================================================================================================================================================================================================================================================
================================================================================
I-2_02_PA	PA/PR z Towar-A, Towar-B i storno Towar-A
I-2_02_PR
================================================================================
Wystawić PA/PR na 2 towary, oba z cena 1 PLN: 
- 1,00* Towar-A, 
- 1,00* Towar-B. 
Wystornowac Towar-A.
Platnosc gotowka w kwocie 1 PLN.
Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).

1. Wprowadzać komenda po komendzie
```
{ "commandType": 16 }
```
```
{ "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "szt" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }
```
```
{ "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-B", "price": 1, "ptu": "B", "unit": "szt" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }
```
```
{ "commandType": 22, "commandInput": { "item": { "advanceRemain": 0, "canceled": true, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "szt" }, "type": 1 }, "print": true, "returnModel": false, "returnPDF": false }
```
```
{ "commandType": 24, "commandInput": { "name": "paymentName", "payment_type": 1, "value": 1, "payment_without_terminal": true } }
```
```
{ "commandType": 26, "commandInput": { "canceled": false }, "print": true, "returnPDF": false, "returnQR": true }
```
=============================================================================================================================================================================================================================================================================================================
================================================================================
I-2_03_PA	PA/PR z Towar-A i narzutem do pozycji i z reszta
I-2_03_PR
================================================================================
Wystawić PA/PR na 1,00* Towar-A, z cena 1 PLN, zastosowac narzut 5 PLN do pozycji.
Platnosc gotowka w kwocie 6 PLN, wplata 10 PLN (oczekiwana reszta 4 PLN).
Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).
1. komenda do wprowadzenia
```
{ "commandType": 30, "commandInput": { "1": {"commandType": 16}, "2": { "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "", "discount": {"name": "Narzut", "type": 1, "unit": 1, "value": 5} }, "type": 1 }, "commandType": 22, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandInput": { "name": "paymentName", "payment_type": 1, "value": 10, "payment_without_terminal": true }, "commandType": 24 }, "4": {"commandType": 26} } }
```
2. dla PA
```
{ "commandType": 30, "commandInput": { "1": {"commandType": 16}, "2": { "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "", "discount": {"name": "Narzut", "type": 1, "unit": 1, "value": 5} }, "type": 1 }, "commandType": 22, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandInput": { "name": "paymentName", "payment_type": 1, "value": 10, "payment_without_terminal": true }, "commandType": 24 }, "4": {"commandType": 26, "commandInput": {"canceled": true}, "print": true, "returnPDF": false, "returnQR": true } } }
```
=============================================================================================================================================================================================================================================================================================================
================================================================================
I-2_04_PA	PA/PR z Towar-C i opustem od pozycji i z reszta
I-2_04_PR
================================================================================
Wystawić PA/PR na 9,00* Towar-C, z cena 1 PLN, zastosowac opust 3 PLN od pozycji.
Platnosc gotowka w kwocie 6 PLN, wplata 10 PLN (oczekiwana reszta 4 PLN).
Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).
```
{ "commandType": 30, "commandInput": { "1": {"commandType": 16}, "2": { "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 9, "name": "Towar-C", "price": 1, "ptu": "C", "unit": "", "discount": {"name": "Opust", "type": 0, "unit": 1, "value": 3} }, "type": 1 }, "commandType": 22, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandInput": { "name": "paymentName", "payment_type": 1, "value": 10, "payment_without_terminal": true }, "commandType": 24 }, "4": {"commandType": 26} } }
```
=============================================================================================================================================================================================================================================================================================================
================================================================================
I-2_05_PA	PA/PR z Towar-A, TOWAR-B i narzutem do podsumy
I-2_05_PR
================================================================================
Wystawić PA/PR na 2 towary, oba z cena 1 PLN:
- 1,00* Towar-A,
- 1,00* Towar-B.
Zastosowac narzut 5 PLN do podsumy.
Platnosc gotowka w kwocie 7 PLN.
Wystawić 2x PA: z podsumowaniem i bez podsumowania (jezeli to mozliwe).
1. komenda do wprowadzenia
```
{ "commandType": 30, "commandInput": { "1": {"commandType": 16}, "2": { "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-A", "price": 1, "ptu": "A", "unit": "" }, "type": 1 }, "commandType": 22, "print": true, "returnModel": false, "returnPDF": false }, "3": { "commandInput": { "item": { "advanceRemain": 0, "canceled": false, "count": 1, "name": "Towar-B", "price": 1, "ptu": "B", "unit": "" }, "type": 1 }, "commandType": 22, "print": true, "returnModel": false, "returnPDF": false }, "4": { "commandInput": { "name": "Narzut", "discount_type": 1, "discount_unit": 1, "value": 5 }, "commandType": 25 }, "5": { "commandInput": { "name": "paymentName", "payment_type": 1, "value": 7, "payment_without_terminal": true }, "commandType": 24 }, "6": {"commandType": 26} } }
```
