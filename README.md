# WPFThreads

OBBIETTIVO: realizzare un conteggio con 3 TextBlock WPF che facevano vedere l'incremento di 3 contatori differenti.

Il primo contatore parte ogni millisecondo e conta fino a 5000, il secondo parte ogni 10 millisecondi e conta fino a 500 e il terzo parte ogni 100 millisecondi e conta fino a 50. Ogni contatore per arrivare alla sua cifra ci mette 5 secondi.

Per far si che i thread contatori partano ci occorre un bottone.

SPIEGAZIONE CODICE:

![AAAAAAA](https://github.com/1bianco9/WPFThreads/assets/116873906/818c344e-8a15-4a47-9679-133168d96fa9)
Per prima cosa andiamo a dichiarare le nostre variabili:
-GIRI 1/2/3 sono le variabili che contengono i vari valori a cui i rispettivi contatori dovranno arrivare
-counter 1/2/3 sono i contatori che scorreranno fino al loro rispettivo numero
-T1/2/3 sono le costanti di tempo che contengono i millisecondi di ciascun giro 

![sema](https://github.com/1bianco9/WPFThreads/assets/116873906/8d24610d-d010-408c-af26-170f395dedcb)
Successivamente dobbiamo inizializzare un semaforo, il semaforo potra' assumere 2 funzioni:
-wait() che sarebbe una procedura bloccante
-signal() decrementa il contatore e quando arriva a 0 si ferma
il semaforo inoltre non potrà assumere valori negativi.

![i1](https://github.com/1bianco9/WPFThreads/assets/116873906/c22f9ade-d747-42c9-8ef8-055612b97012) ![i2](https://github.com/1bianco9/WPFThreads/assets/116873906/a0f8fe5a-7896-473b-a2de-6334e762b21a)






