# Taking Bot

A machine learning based bot designed to have simple conversions with humans. It uses Transfer Learning to build a State-of-the-Art dialog agent based on OpenAI's GPT-2 Transformer language model.

The idea behind this approach is quite simple:
Start by pretraining a language model on a very large corpus of text to be able to generate long stretches of contiguous coherent text,
fine-tune this language model to adapt it to our end-task: dialog.

The model is given a prior consisting of part of a conversation.
Then the network generates one paragraph to complete one answer in the conversation.
Next we can add our own response and the cycle repeats.

The ability to recognise and give output speech is also added using open-source models and libraries.

<br>

## Below are exerpts from some of the conversations with the bot:

**When trained for  general conversations:**

**Bot**: "Nice to meet you. What's your name?"

**Human**: "My name is Atharva."

**Bot**: "That's an interesting name."

**Human**: "Can you tell me something about yourself?"

**Bot**: "Of course! I like playing video games"

**When trained on a science-fiction movies dataset:**

**Human**: "Do you like science fiction?"

**Bot**: Yeah, I like science fiction. It's a wonderful story that I enjoy. Everything about it is fascinating, and you guys are a great bunch.

**Human**: "I've watched every Star Trek movie."

**Bot**: "Yeah. Star Wars, Spielberg, All the Star Technical Stuff. I watch every Star Trek film."

**Human**: "Do you think the warp engine could really exist one day?"

**Bot**: "Eh, no, I doubt you."



## Usage Guide
The '**dataset.txt**' file is the dataset used to train the bot. You can use your own dataset provided it is in the format of the original file.

The '**training.ipynb**' file is the Python program used to train the bot. It is recommended to run this using Google Colab to avoid any errors or modify the file appropriately to run it locally.

The '**run_bot.ipynb**' file is used to run the bot after training it. This directory which contains this file should also contain the checkpoints for the model trained using the previous program. Since access to microphone and speakers is required here, it is recommeded to run this program locally after downloading the checkpoint files from Colab.

 
