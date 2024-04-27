Sono presenti tre diversi notebook: uno per effettuare il fine tuning,uno per generare le risposte con il modello con il fine tuning, ed infine uno per effettuare la valutazione per span
I notebook sono usabili sia con il modello T5 sia con il modello FLAN T5

Il notebook del fine tuning è già predisposto e configurato per essere avviato, bisogna cambiare i path dei dataset di train e di validation, il path della directory in cui vengono salvati tutti i vari checkpoint del modello con il fine tuning ed eventualmente il nome del modello scelto: i modelli disponibili con il flan t5 sono disponibili al seguente link: https://huggingface.co/docs/transformers/model_doc/flan-t5
mentre quelli con il t5 sono disponibili al seguente link: https://huggingface.co/docs/transformers/model_doc/t5
E' possibile modificare anche i parametri globali del training a seconda della necessità, come per esempio la dimensione dei batch affinchè il modello sia caricato correttamente nella VRAM della gpu disponibile.

Il notebook per generare le risposte presenta due alternative: è possibile generare una singola risposta tramite la funzione generate_question passando come parametri una stringa contenente la frase da dare in input e il path contenente il modello con il fine tuning; nell'altra cella è possibile invece generare un file json contenente tutte le risposte che il modello genera tramite un test set; è necessario cambiare i vari path del dataset, del modello con il fine tuning e della directory dove salvare il risultato

Tramite l'ultimo notebook invece è possibile generare la valutazione sul test set tramite span con il tipo: è necessario solamente passare alle due funzioni i path del file del dataset e quello dei risultati e le funzioni si occuperanno di calcolare le metriche.
E' necessario prima avviare la prima cella per far si che le rimanenti funzioni eseguano tutto correttamente.


Nella cartella sono già presenti i file con il dataset: sono presenti i file di training, validation e test set in 3 diverse versioni: una con incapsulamento, uno senza incapsulamento ed uno senza differenze(in cui sono incluse le altre due versioni)