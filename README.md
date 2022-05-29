# UrduFake-FIRE-2021

Submission for the UrduFake track in FIRE 2021

Dataset used - 'Bend the Truth'

We have used four transformer based models (only the encoder part). We fine-tuned the pre-trained models from [huggingface]([url](https://huggingface.co/)) on our dataset. One additional output layer is added to calculate the probability of real and fake classes. Two monolingual (roBERTa and ALBERT) and two multilingual (XLM-RoBERTa and Multilingual BERT) models have been used. After hyperparameter tuning using Raytune, different combinations were ensembled using soft-voting. 


<img width="495" alt="image" src="https://user-images.githubusercontent.com/54231666/170870783-70cc6f18-34db-4840-9314-88022761e44a.png">

The multilingual models and ALBERT gave very poor results. 
