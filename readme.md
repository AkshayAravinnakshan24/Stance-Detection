Stance-Detection using Hugging Face GPT2
GPT2
GPT-2 is a direct scale-up of GPT, with more than 10X the parameters and trained on more than 10X the amount of data. GPT-2 is a large transformer-based language model with 1.5 billion parameters, trained on a dataset of 8 million web pages. GPT-2 is trained with a simple objective: predict the next word, given all of the previous words within some text. I have added two more dense layers to this state of art model and converted it to perform Stance classification on twitter data. 

PRE-REQUISITES:

pip install transformers
pip install torch
pip install numpy as np
pip install pandas as pd

USING THE MODEL

I have fine-tuned the Hugging face English GPT2 model on Tesla T4 Azure VM. I have also open sourced the fine-tuned model. I order to see the working of this model please use the following steps.
Step 1. Clone the repository with the following files.
Step 2. Replace the tweet variable with any desired tweet. (You can also provide urls, Hastags, and special charecters )
Step 3. The model downloads all the requisites and prints the ‘Stance’ of the tweet and with its ‘probability score’
!pip install import-ipynb
import import_ipynb,StarStancePredictor
from StarStancePredictor import Star_Stance_Model
tweet= ‘Crazy: ‘Patagonia's viral 'vote the #assholes out' tags are real! 
Read more on: https://t.co/N2fa0MxlOG
#patagonia #viral #VoteThemAllOut2020 #VoteHimOut #VoteHimOut2020 #VoteReady #VoteThemOut #VoteTrumpOut #VoteTheAssholesOut #AssholesLiveForever #votetosaveamerica #Hayvine https://t.co/rEn5uEs8io’
StarStancePredictor.Star_Stance_Model(tweet)

