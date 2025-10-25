---
author: Bronwen Aker
updated: 2025-09-30
presentation_type: Workshop
venue: WWHF - Deadwood
---
```table-of-contents
title: # Table of Contents
minLevel: 0
maxLevel: 3
```

# Time for Some History

If you haven't been involved in technology and technology innovation for a long time, say decades, you might not be aware that artificial intelligence has been around for a very long time.

Using ChatGPT, I generated this timeline of events from the time the term "artificial intelligence" was first coined through present day.

- **1956** – John McCarthy coins the term _Artificial Intelligence_ at the Dartmouth Conference.    
- **1960s–70s** – Early symbolic AI and “expert systems” emerge, but limited by computing power.    
- **1980s** – Expert systems gain traction in business; AI winter follows due to cost and limitations.    
- **1997** – IBM’s _Deep Blue_ defeats world chess champion Garry Kasparov.    
- **2000s** – Machine learning and statistical approaches begin outperforming symbolic AI.    
- **2012** – Breakthrough in deep learning with AlexNet winning ImageNet competition.    
- **2016** – Google DeepMind’s _AlphaGo_ defeats Go champion Lee Sedol.    
- **2020s** – Rapid advances in generative and large-scale AI:    
    - **2020** – OpenAI releases GPT-3, showing unprecedented natural language generation.        
    - **2021** – Codex powers GitHub Copilot, bringing AI-assisted coding into mainstream use.    
    - **2022** – Diffusion models (e.g., DALL·E 2, Stable Diffusion, MidJourney[^1]) popularize AI image generation.        
    - **2022** – ChatGPT launches, sparking global awareness of conversational AI.        
    - **2023** – OpenAI releases GPT-4, expanding multimodal capabilities (text and images).        
    - **2023–24** – Major tech firms integrate AI assistants into office tools, search engines, and operating systems.        
    - **2024–25** – Growth of open-source LLMs (LLaMA, Mistral, Falcon, etc.) alongside enterprise-grade AI governance and safety research.        

#### TL;DR
AI, first defined in 1956, has progressed from symbolic reasoning to machine learning and deep learning, experiencing multiple cycles of hype and disappointment. Recent advances in large-scale generative and multimodal models have brought widespread adoption, alongside significant concerns over accuracy, bias, security, and governance.

## Ok, So What IS It?!?
 Simply put, AI is a vast discipline within computer science aimed at creating systems to perform tasks that we normally think of as requiring human intelligence to perform. AI includes fields like robotics, computer vision, natural language processing (used to translate voice to text and vice versa), expert systems, etc.

In a very real way, the technologies developed for handling and analyzing large quantities of data paved the way for what we currently call artificial intelligence.[^2] 
 
![[AI Venn.png]]

## Where Do LLMs Fit In?
LLMs Are a subset of generative AI. LLM only deal with text, whereas diffusion models deal with imagery. LLMs are probabilistic, which is a fancy way of saying that everything they "create" is generated based on probabilities. How likely it is that you're going to get one answer versus another depends on not just what your prompt was, but also on a lot of math that goes on both inside the model and in the supporting the software that helps you interact with it.[^3]

The current trend with the innovators in LLM development is to follow the "bigger is always better" headspace, training their proprietary models on massive amounts of data from diverse sources. Not surprisingly, most of the LLMs you will find available (ChatGPT, Claude, Copilot, Gemini) are general purpose. You can use them for anything from learning more about a historical concept to finding the perfect rice pudding recipe. You can also do some limited customization (e.g., Custom GPTs), But you are limited to whatever customization features are being provided by the AI provider. More importantly for a lot of people, anytime you use one of these hosted chat bots, you have no control over what happens to your data once you send it across to them.

Regardless, easy access to large language models and their chatbots has popularized artificial intelligence more than ever before.

## Why Go Local?
 When I talk to people about why they want to set up and customize a local LLM, the number one reason they cite is privacy. When you host your own LLM, no data ever has to leave your machine, network, or intranet. All of your sensitive files and data remain in your control.

Also, hosting your own local LLM gives you many more options for customizing and fine tuning a model to suit your needs. You can create custom models using a very simple process that we will do ourselves in the Ollama lab. Other options for customization and data handling include Retrieval-Augmented Generation (RAG), or you can train your own model from the ground up. Be forewarned, if you choose to go that route it is a very, *very* deep rabbit hole!











[^1]: For the record, Midjourney was my gateway drug into AI. https://www.midjourney.com/

[^2]: I personally hate the term "artificial intelligence" because, 1) since these are digital tools it should be obvious that they're artificial, and 2) the reality is that they are anything but intelligent. 

[^3]: As previously mentioned, if you want to get really deep into the weeds about the data science of how LLMs work, check out *[AI for Cybersecurity Professionals with Joff Thyer and Derek Banks](https://www.antisyphontraining.com/product/ai-for-cybersecurity-professionals-with-joff-thyer-and-derek-banks/)*. 
