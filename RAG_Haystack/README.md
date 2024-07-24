# README.md

## Purpose

Exercise in basic Retrieval Augmented Generation (RAG) system coding (using only fully open source tools only).
In this simple example, the agent is created to be an expert on shoes sold on an online shoe store. If you ask it
questions about the range of shoes sold, it should answer only with the information supplied.

## Environment Setup

Create a virtual environment, call it '.venv'.

```
python3 -m venv .venv
```

Activate it.

```
source .venv/bin/activate
```

Get pip and install it.

```
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py
```

Get the required packages for this project (this may take a while):

```
pip install -r requirements.txt
```

NOTE: some of the required pip packages are enourmous. In order to get it to work and avoid the dreaded 'No space left on device' error. You may need to point pip at a directory with more space available, I used a tmp directory in my home folder. run this first, then try again:

```
export TMPDIR=$HOME/tmp
```

## Model Installation

The model is too large to check in to github (and it would be rather a waste of space), so is not checked in. Consequently, you will need to download it from HuggingFace, here: https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF/blob/main/llama-2-7b-chat.Q5_K_S.gguf - place it in the models folder.

## Running

Open the RAG_Pipeline.ipynb in Jupyter. Run all. Try changing the question...
![image](https://github.com/user-attachments/assets/d6d25391-298a-41a7-a5f4-79914ff7c032)

## Notes

This will run on 'bare metal' (the CPU) by default. Follow instructions on the llama.cpp installation page to install llama-cpp-python for your preferred compute backend if you wish to change this to use your GPU, for instance.
