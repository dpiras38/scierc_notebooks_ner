There are three different notebooks: one for fine-tuning, one for generating responses with the fine-tuned model, and the last one for evaluation based on span.

The fine-tuning notebook is already set up and configured to be run. You need to change the paths for the training and validation datasets, as well as the path of the directory where all the various fine-tuned model checkpoints will be saved. It is also possible to modify global training parameters as needed, such as batch size, to ensure that the model is properly loaded into the available GPU VRAM.

The response generation notebook offers two alternatives: in the first cell, you can generate a single response by modifying the example string in the "question" variable, which contains the sentence from which entities should be extracted. Lastly, you need to change the path to the fine-tuned dataset. In the other cell, you can generate a JSON file containing all the responses the model generates using a test set. You need to change the paths for the dataset, the fine-tuned model, and the directory where the results will be saved.

The last notebook allows you to generate an evaluation on the test set using span-based evaluation. You only need to provide the file paths for the dataset and results, and the functions will calculate the metrics.

The folder already contains the dataset files: there are training, validation, and test set files in three different versions: one with encapsulation, one without encapsulation, and one without differences (which includes the other two versions).
