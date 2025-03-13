There are four notebooks: one for fine-tuning, one for generating responses with the fine-tuned model, one for span-based evaluation, and one for generating responses using zero and few-shot learning and extracting them correctly.

The fine-tuning notebook is already set up and configured to be run. You need to change the paths for the training and validation datasets, as well as the path of the directory where all the various fine-tuned model checkpoints will be saved. You can also modify the global training parameters as needed, such as batch size, to ensure that the model is properly loaded into the available GPU VRAM.

The response generation notebook offers two options: in the first cell, you can generate a single response by modifying the example string in the "question" variable, which contains the sentence from which entities should be extracted. Lastly, you need to change the path to the fine-tuned dataset. In the other cell, you can generate a JSON file containing all the responses the model generates using a test set. You need to change the paths for the dataset, the fine-tuned model, and the directory where the results will be saved.

The evaluation notebook allows you to generate an evaluation on the test set using span-based evaluation. You only need to provide the file paths for the dataset and results, and the functions will calculate the metrics.

The zero/few-shot notebook differs from the classic one by the presence of several prompts and some modifications to the entity extraction function from the predictions, to handle cases that do not occur with other models.

The folder already contains the dataset files: there are training, validation, and test set files in three different versions: one with encapsulation, one without encapsulation, and one without differences (which includes the other two versions).