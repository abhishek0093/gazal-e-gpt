# Gazal-e-GPT  

## Background  
I've always been fascinated by how poets and writers beautifully express their thoughts through poems and stories. Honestly, I wasn’t very good at it myself—but with the rise of GenAI, that doesn't matter anymore. So I decided to create something that could write better than me: Gazal-e-GPT.  

Instead of just fine-tuning a pre-trained model (which would’ve been easier), I took it as a learning opportunity. I built the entire GPT model from scratch, coding every layer and connection and then training it step by step.  

## Training Process  
Since I was limited by my MacBook Pro and MPS device support, training was slow. But with a few tweaks, Google Colab offered a much better performance.  

## Dataset  
For Hindi-Urdu ghazal-style text, there isn't much data available. I used the dataset from [this repo](https://github.com/amir9ume/urdu_ghazals_rekhta), focusing only on Hindi versions for now.  
The dataset is around 2MB, which is small compared to the model size. Increasing the dataset size would definitely improve the model’s performance.  

## Training Graphs  
![image](https://github.com/user-attachments/assets/8f1cfd16-15b4-4a8e-86cc-59df2ce363f1)  
![image](https://github.com/user-attachments/assets/ad55f13f-5f9f-4931-94a4-4639f7f42c03)  
![image](https://github.com/user-attachments/assets/8ab3b8a5-f8c4-4464-a163-f3cdd082b61e)  

## Outputs  
**User Input:** चलो आज फिर चलते हैं  
**Epoch-1 Model Output:** खुदा से ये गुजारिशમે साला<<reserved_token_3325>> Agency<<reserved_token_4075>> ਲੰਬਾ ਜਾਣਕਾਰੀ ਨਿਰਧਾਰਤ ਮੌਜੂਦsd റൂ females females AT ವ್ಯವಹ Illహంpret<<reserved_token_2098>> dietsm गोष्टी used વેપ ਗਵਰਨਰસંગતitory ವ್ಯವಹನಿಯನ್ गोंൃതിसंबंध British ਪਾਲ খেলেনটো ನಿರ್ವಹಿಸಲುसतनਗਤ<<reserved_token_2313>>ಬರ್ pictures


**Epoch-800 Model Output:** चलो आज फिर चलते हैं सुनते थे दिल की आग उस की तबी दयारों पे हम भी अब दादे हैं तो जी बहकी रुफ़ाई है पयाम रख देंगी गुज़राज़ारे लोग मिले भी अब तक लेकिन एक दिलबर नहीं है उल्फ  

## Future Improvement Plans  
* The current tokenizer is from [Sarvamai](https://huggingface.co/sarvamai/sarvam-1). While it's great for Indic languages, it's not specifically designed for Urdu, which impacts performance.  
* Increasing dataset size and using CUDA for faster training.  
* Pretraining on general Hindi-Urdu text and poetic data, followed by fine-tuning with ghazal-style text to better align outputs to desired gazals style.  

## References  
* [GPT-2](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) and [GPT-3](https://arxiv.org/abs/2005.14165) research papers  
* [OpenAI's GPT-2 Repo](https://github.com/openai/gpt-2)  
* [Andrej Karpathy](https://karpathy.ai/) and his [YouTube videos](https://www.youtube.com/watch?v=l8pRSuU81PU)  
