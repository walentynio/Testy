# Testy
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
