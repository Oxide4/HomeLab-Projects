
---

# Local AI Chatbot Project

I wanted to challenge myself by running a localized AI chatbot directly on my laptop.
(The laptop I used for this can be found here: [Refurbished Laptop Project](https://github.com/Oxide4/HomeLab-Projects/tree/main/Refurbished-Laptop))

This project was mainly for me to learn more about how AI chat models work, and to get more hands-on experience with Linux and some new tools. While I built this for personal learning, I’ll walk through the steps in case anyone else wants to try something similar.

---

## What I Did (And How You Can Do It Too)

### 1. Update Your System

First, I made sure everything on my system was up to date. If you're doing this yourself, open a terminal and run:

```bash
sudo apt update
```

### 2. Install Ollama

Next, I installed **Ollama**, a tool that lets you run AI models locally. Here’s the install command I used:

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

Depending on your hardware, this might take a bit. On my laptop, it took a while so just be patient.

### 3. Check That It’s Running

To make sure Ollama installed correctly, I opened a browser and went to:

```
localhost:11434
```

If everything is working, you’ll see a message that says: **Ollama is running**.

### 4. Install a Chat Model (I Picked LLaMA 3)

I wanted to try out Meta’s LLaMA 3 model. To download it, I used this command:

```bash
ollama pull llama3
```

This step also took a bit of time on my hardware, but once it's done, you’re ready to go.

### 5. Run the Chatbot

To start chatting with the model, just type:

```bash
ollama run llama3
```

That will launch the chatbot. It works just like any other AI chatbot you’ve used online, except now it’s running entirely on your own machine.

To end the session, type:

```
/bye
```

---

## Conclusion

This project was a great way for me to learn more about AI models and get more familiar with Linux at the same time. I definitely ran into some slowdowns because my laptop isn’t super powerful, especially when it comes to the GPU. The bot takes some time to think and respond, but honestly, I expected that.

I plan to keep working on this project. I’d like to improve the UI, and maybe eventually run this setup on a dedicated server instead of my laptop.

Even though this was mostly for me, I think it’s a fun and educational project that others might enjoy too. If you're curious about how AI models work under the hood, give it a try but just don’t expect lightning speed if you're running it on older hardware like I am.

---
