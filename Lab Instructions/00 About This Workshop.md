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

# Welcome

Thank you for signing up for the WWHF Deadwood 2025 Edition of *Keeping Things Local: How to Set Up and Customize Your Own LLM*. I'm your host, Bronwen Aker, aka Corvus, aka The Cybrarian. 

The world of artificial intelligence (AI) is complex and confusing, especially because there is so much hype. There is also a lot of good information available, through YouTube, through online courses, and through events like this, but it can still feel overwhelming when you're starting to learn about how AI works and what its limitations are. This workshop covers a lot of the fundamentals, and introduces you to some of the easier, yet still very effective, ways that you can customize an existing model to suit your own needs. 

## Additional AI Training from Antisyphon

If you want to get deeper into the weeds, learning about the math underneath all this stuff, check out *[AI for Cybersecurity Professionals with Joff Thyer and Derek Banks](https://www.antisyphontraining.com/product/ai-for-cybersecurity-professionals-with-joff-thyer-and-derek-banks/)*. Joff and Derek cover foundational AI history, concepts, and data science underpinnings. They also address various statistical approaches in use by AI and machine learning, including regression techniques, support vector machines, gradient boosting algorithms, and more.[^1] 

https://www.antisyphontraining.com/product/ai-for-cybersecurity-professionals-with-joff-thyer-and-derek-banks/

And if you are all about the Red Team, check out *[Exploiting AI with Ben Bowman](https://www.antisyphontraining.com/product/exploiting-ai-with-ben-bowman/)*. Ben starts his course with the assumption that students have very little about AI beyond how to use tools like ChatGPT. Then he starts with the basics: how AI behaves, key concepts, and essential terminology in the field. Once that foundation is in place, the focus shifts to exploring attack surfaces through hands-on labs and practical examples.

https://www.antisyphontraining.com/product/exploiting-ai-with-ben-bowman/



# What to Expect

I've broken the material down into several different lessons, starting with setup, then some AI/LLM basics, and moving on to more complicated material as we progress. 
### Tools We Will Be Using

* VMware Virtual Machine (Workstation or Fusion)
* Ollama (pre-installed)
	* Selected LLM models
	  The virtual machines are already loaded with Olama and fairly small sized LLM models to ensure that they are usable, even on a laptop that doesn't have the best system resources. GPUs are really nice, but they are not absolutely necessary when it comes to using LLM models that are already configured. (There's also this little problem about them being gigabytes large per file, and we are already stressing the Wi-fi here in Deadwood. Preloading the LLM models avoids all that trouble.)
* Msty (pre-installed)
  Msty is used to compare the interactions of more than one LLM at a time. This can be handy when fine-tuning a customization. 

### [[01 What is an LLM]]
First, we will cover some of the fundamentals, doing a brief and high level overview of the history and recent innovations in artificial intelligence technologies, and helping students become acquainted with fundamental terminology used here and in other AI courses.
### [[02 Setting Up Your VM]]
The virtual machine we will be using for this workshop has already been built for you. You will, however, need to have VMware installed on a host system. If you've never worked with a VM before, this page will walk you through getting the VM set up.
### [[03 Working With Ollama]]
Ollama is an excellent introduction to working with local Large Language Models (LLMs). Its native interface is command line (CLI), but it's easy to set up a local web server instance so you can chat with it using a browser. Other programs, like Msty, can also connect to Ollama or other LLM models, but more about that later.
### [[04 Using Msty]]
Once you have worked with Ollama a bit and created your first custom LLM model, it's time to use Msty to compare the performance of the original model with your new one. 




[^1]: This class is best for students who already have experience using the Python programming language, and who are already familiar with basic statistical concepts. 
