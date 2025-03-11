There are three different types of notebooks: one for fine-tuning, one for generating responses with the fine-tuned model, and one for evaluation.

The fine-tuning notebook is already set up and configured to be run. You need to change the paths for the training and validation datasets, the path of the directory where all the various fine-tuned model checkpoints will be saved, and, if necessary, the name of the selected model. For SciBERT, "allenai/scibert_scivocab_uncased" was used, while for SciDeBERTa, "KISTI-AI/scideberta-cs" was used.

The notebook is already set up and configured to be run; it is necessary to change the various paths for the fine-tuned model's dataset and the directory where the result will be saved, as well as the training arguments.

The main folder already contains the dataset files: there are training, validation, and test set files in three different versions—one with encapsulation, one without encapsulation, and one without differences (which includes the other two versions but is not used for SciBERT).
