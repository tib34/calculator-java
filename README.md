Numărul total de linii de cod (LOC) pentru întregul proiect:
•	Total LOC: 124

Complexitatea Ciclomatică și Cognitivă
Metoda evaluateExpression

Complexitate Ciclomatică:
•	Număr de blocuri de control: 4 (if, for, if, switch)
•	Complexitate ciclomatică totală: 5 (1 pentru metoda de bază + 4 blocuri de control)
Complexitate Cognitivă:
•	Estimativ: 6 (blocuri if, for, switch și operații de stivă)

Metoda Calculate
Complexitate Ciclomatică:
•	Număr de blocuri de control: 1 (switch)
•	Complexitate ciclomatică totală: 2 (1 pentru metoda de bază + 1 switch)
Complexitate Cognitivă:
•	Estimativ: 3 (bloc switch și cazuri multiple)
Plan de Testare Black Box
1. Testare cu Operații Simple
•	Intrare: "3+2"
o	Ieșire Așteptată: "5.0"
o	Motivare: Adunarea simplă a două numere.
•	Intrare: "5-2"
o	Ieșire Așteptată: "3.0"
o	Motivare: Scăderea simplă a două numere.
•	Intrare: "4*3"
o	Ieșire Așteptată: "12.0"
o	Motivare: Înmulțirea simplă a două numere.
•	Intrare: "8/4"
o	Ieșire Așteptată: "2.0"
o	Motivare: Împărțirea simplă a două numere.
2. Testare cu Operații Mixte
•	Intrare: "2+3*4"
o	Ieșire Așteptată: "14.0"
o	Motivare: Înmulțirea are prioritate față de adunare.
•	Intrare: "10/2-1"
o	Ieșire Așteptată: "4.0"
o	Motivare: Împărțirea se efectuează înainte de scădere.
•	Intrare: "5*(2+3)"
o	Ieșire Așteptată: "25.0"
o	Motivare: Parantezele schimbă ordinea operațiilor.
•	Intrare: "3+5*2-8/4"
o	Ieșire Așteptată: "9.0"
o	Motivare: Se respectă ordinea operațiilor: înmulțire și împărțire înainte de adunare și scădere.
3. Testare cu Expresii Complexe
•	Intrare: "10-2*5/2"
o	Ieșire Așteptată: "5.0"
o	Motivare: Înmulțirea și împărțirea se efectuează înainte de scădere.
•	Intrare: "100/(5*2)-3"
o	Ieșire Așteptată: "7.0"
o	Motivare: Înmulțirea este efectuată înainte de împărțire și scădere.
4. Testare cu Inputuri Speciale
•	Intrare: "0+0"
o	Ieșire Așteptată: "0.0"
o	Motivare: Verifică comportamentul cu zero.
•	Intrare: "-3+5"
o	Ieșire Așteptată: "2.0"
o	Motivare: Adunarea unui număr negativ cu un număr pozitiv.
•	Intrare: "5/0"
o	Ieșire Așteptată: "ERROR"
o	Motivare: Împărțirea la zero ar trebui să returneze o eroare.
•	Intrare: "Infinity+1"
o	Ieșire Așteptată: "Infinity"
o	Motivare: Verifică tratarea valorilor infinite.
5. Testare cu Inputuri Invalid
•	Intrare: "5++3"
o	Ieșire Așteptată: "ERROR"
o	Motivare: Verifică comportamentul pentru sintaxa invalidă.
•	Intrare: "a+2"
o	Ieșire Așteptată: "ERROR"
o	Motivare: Verifică comportamentul pentru caractere non-numerice.
•	Intrare: "5+2*"
o	Ieșire Așteptată: "ERROR"
o	Motivare: Verifică comportamentul pentru operații incomplete.

Revizuire Informală și Analiză Statică
Observații Generale:
•	Codul este curat și bine structurat.
•	Metodele sunt definite clar și sunt ușor de înțeles.
•	Utilizarea stivei pentru evaluateExpression este eficientă pentru evaluarea expresiilor postfixate.

Sugestii de Îmbunătățire:
•	Documentație: Adăugarea comentariilor Javadoc pentru metode și explicații suplimentare în cod ar putea îmbunătăți ușurința înțelegerii.
•	Gestionarea Erorilor: În metoda calculate, ar fi util să se gestioneze mai bine erorile pentru operatorii invalizi sau diviziunea prin zero.
