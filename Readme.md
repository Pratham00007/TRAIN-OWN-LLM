# CodeCamp.org Course

# Train language model & evolution of the Transformer architecture courses

We’ve all used Large Language Models (LLMs) and been amazed by what they can do. I wanted to understand how these models are built, so I created this course.

I’m from Morocco and speak Moroccan Darija. Most LLMs today understand it a little, but they can't hold proper conversations in Darija. So, as a challenge, I decided to train a language model from scratch using my own WhatsApp conversations in Darija.

I've made a YouTube playlist documenting every step. You can watch it at your own pace. If anything is unclear, feel free to open an issue in this repository. I’ll be happy to help!



In the first course, I used the Transformer architecture that was introduced in 2017. It is 2025 now, and the Transformer architecture has evolved significantly since then. So, I created a second course to explain the evolution of the Transformer architecture and how to implement some of the recent advancements.


## What is in this repository?

- `notebooks/`: Jupyter notebooks for each step in the pipeline.
- `Slides.odp & Slides.pdf`: Presentation slides used in the YouTube series.
- `data/`: Sample data and templates.
- `transformer/`: Scripts for the Transformer and LoRA implementations.
- `minbpe/`: A tokenizer from [Andrej' Karpathy's repo](https://github.com/karpathy/minbpe), since it's not available as a package.
- `RESOURCES.md`: List of resources and references.

## Setup

To get started, install [Python](https://www.python.org/downloads/) and the required dependencies by running:  

```bash
pip install -r requirements.txt
```

## What I learned?

### Train language model from scratch course

This course covers:  

1. Extracting data from WhatsApp.  
2. Tokenizing text using the BPE algorithm.  
3. Understanding Transformer models.  
4. Pre-training the model.  
5. Creating a fine-tuning dataset.  
6. Fine-tuning the model (Instruction tuning and LoRA fine-tuning).  

Each topic has a video in the [YouTube playlist](https://www.youtube.com/playlist?list=PLMSb3cZXtIfptKdr56uEdiM5pR6HDMoUX) and a Jupyter notebook in the [`notebooks/`](./notebooks/) folder.

### Evolution of the Transformer architecture course

This course covers:

1. Various techniques for encoding positional information  
2. Different types of attention mechanisms  
3. Normalization methods and their optimal placement  
4. Commonly used activation functions  
5. And much more

Each topic has a video in the [YouTube playlist](https://www.youtube.com/playlist?list=PLMSb3cZXtIfphv0UD9juixGhCZZRvlBAj) and a Jupyter notebook in the [`notebooks/`](./notebooks/) folder.

## My experience

### Course 1

Like you, I had never trained a language model before. After following the steps in this course, I built my own 42M parameter model called **BoDmagh**. In Moroccan Darija, **BoDmagh** can mean **someone with a brain**. The word **Bo + [noun]** means something is deep inside you, so **BoDmagh** can also mean a smart person.

### Course 2

After completing this second course, I compared the performance of the original Transformer model with a modified version that incorporates some of the advancements discussed in the course. I found that these new ideas siginificantly enhanced the Transformer architecture across various aspects such as memory usage, inference speed, better results, etc.

This graph shows the validation loss improving after applying one idea at a time:


Seeing this improvement made me very happy because it confirmed that these advancements are effective and beneficial.

### Limitations  

The model we trained in the first course doesn’t always give correct answers. If I try to discuss many different topics, it struggles. This is likely because both the model and the SFT dataset are small. Training on more data and using a larger model could improve the results. I might explore this in the future.
