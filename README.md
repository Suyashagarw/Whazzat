# Whazzat

The Whazzat project is aimed at developing a sophisticated product recommendation system to alleviate the common challenge users encounter when searching for products that precisely meet their needs. Many users struggle to articulate their product requirements clearly, leading to misunderstandings and inefficiencies with search platforms. Whazzat addresses this issue by streamlining the search process. It accepts general product descriptions as input and delivers relevant product links as output. For instance, if a user inputs a phrase like "something to dig food," Whazzat responds with product listings, such as forks and spoons, presented as clickable links for convenient purchase. To achieve this, the system leverages the Llama 2 7B Chat model, which is fine-tuned and executed on the free version of Google Colab.

✅ The backend is in nodejs, to make it easier to deploy in Firebase functions.

✅ [Axesso - Amazon Data Service API Documentation (axesso) | RapidAPI] (https://rapidapi.com/axesso/api/axesso-amazon-data-service1/) is used to fetch products from Amazon. 

✅ Appsmith to host our frontend https://app.appsmith.com/app/whazzat/home-6556f707c8bcd467b929daa4 

✅ The dataset is a mix of data collected manually and data synthesized using GPT-4 and MostlyAI

✅ clean_data.py is the script used to clean and structure the raw data

✅ Fine_tune_Llama2_7B.ipynb is the script we use to fine-tune the base mode. QLoRA based PEFT (parameter efficient fine tuning) is used to train the Llama2 model in google colab's free edition.

✅ Fine_tuned_Llama2_evaluation.ipynb is the script that validates the Llama2 output with GPT-3.5-Turbo.

✅ Whazzat.ipynb is the final script which runs the fine-tuned model. A user interface is developed using Gradio.


