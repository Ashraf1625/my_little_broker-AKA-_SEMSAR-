# my_little_broker ( سمسار)
![my_little smsar](https://github.com/user-attachments/assets/ef04a61b-ceca-4157-87a5-e0acb3fd25c0)

**Fine-Tuning the Ollama Model with Unsloth and Deploying via Streamlit**  

Welcome to **My Little Broker**, a project that fine-tunes the Ollama model using **Unsloth** . The fine-tuned model is deployed using **Streamlit** for an interactive and user-friendly experience.

---

## Features  

- **Fine-Tuning with Unsloth**: Tailored the Ollama model to specific tasks using the Alpaca format for data preparation.  
- **Streamlit Deployment**: Simple, accessible web-based interface for model interaction.  
- **Optimized with Accelerate**: Ensures efficient training and inference workflows.  
- **Lightweight Precision Handling**: Incorporates `bitsandbytes` for 8-bit optimization.  

---

## Installation  

To set up the project locally, follow these steps:  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/yourusername/my-little-broker.git  
   cd my-little-broker  

2. install the requirments
   ```bash
   pip install streamlit transformers accelerate scipy bitsandbytes==0.40.0 torch torchvision torchaudio peft  
3. run the app
   ```bash
   streamlit run app.py



# usage 

the main aim for this project is to make searching for an apartment easier and more effiencet instead of the old ways to look for a broker to find you an apartment aka smsar we have trained this model 

llama 3.1 using unsloth as we found it to be more cost effincent as the trainer api from hugging face on the same data will take up to 10 hours on training time which can be lot we used the alpaca fomrat 

to fine tune this model [alpaca fomrat ] ( https://github.com/tatsu-lab/stanford_alpaca) as the llama model uses this format to be able to fine tune it 

we trained this model more of a RAG instead of fine tuning it as we see that is RAG is more effinect . we also collected the data from multiple websites using data scraping libraires like beatiful soap

and then we turned this data into prompts to incrase the data like where can i find [apartment] of [size] located in [location] and we put the values of our data inside this fomrat we have been able to generate up 

to 300000 prompts to train the model 

![WhatsApp Image 2024-10-23 at 04 00 47_66cfcdc4](https://github.com/user-attachments/assets/f8ec9e62-d0ab-4a60-93af-ecdc3cc38fec)


# note

you can install this model on your local machine the only catch if you want to deploy this on a cloud service you should have a cuda support cloud service which we found a very complicated 
and hard thing to find 
