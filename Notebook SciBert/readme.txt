Sono presenti tre tipi diversi notebook: uno per effettuare il fine tuning, uno per generare le risposte con il modello con il fine tuning e uno per effettuare la valutazione.

Il notebook del fine tuning è già predisposto e configurato per essere avviato, bisogna cambiare i path dei dataset di train e di validation, il path della directory in cui vengono salvati tutti i vari checkpoint del modello con il fine tuning ed eventualmente il nome del modello scelto: per scibert è stato utilizzato "allenai/scibert_scivocab_uncased",per scideberta invece "KISTI-AI/scideberta-cs"

Il notebook è già predisposto e configurato per essere avviato, è necessario cambiare i vari path del dataset del modello con il fine tuning e della directory dove salvare il risultato, oltre che i training arguments


Nella cartella principale sono già presenti i file con il dataset: sono presenti i file di training, validation e test set in 3 diverse versioni: una con incapsulamento, uno senza incapsulamento ed uno senza differenze(in cui sono incluse le altre due versioni, non tutilizzata per scibert)