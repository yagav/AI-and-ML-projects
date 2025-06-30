Hello everyone, I have finetuned a LLM using unsloth LLama3.2 pretrained model with vit faculty data. The finetuned model is capable of answers simple question regarding the faculty like, the email id of the faculty, their publications. research areas, and about themselves. 

I had collected the data from the official vit Chennai website and used the help of gemini ai to filter and structure the information in the webpage into a excel file ("vit faculty.csv") with all the necessary information I wanted for training.

To finetune a LLM i need a qa set to make a qa set out the information i made "qa set.ipynb" which gives me a json file full of qa sets ("qa_set.json")

The LLM is now finetuned with the help of the usloth library where Llama 3.2 is used as the base model for training. Then the lora adapters are saved in the folder vit_FineTune_model after training done in "llm_vit_faculty.ipynb" file .

"FTllm_inference.ipynb" is used to load the saved model and run inferences on the model.

Conclusion: This project that craeted a finetuned llama 3.2 model with vit faculty data is answering questions perfectly good, eventhough there are mistakes when asked for a specific information, the model is working good enough to answer general questions about the mentioned faculties in VIT Chennai.

Project made using Google Colab
References: Unsloth documetation
