
# README

A very 'rough and ready' Machine Learning notebook thing I've been working on.

See 'Learn AI with Python' by Gaurav Leekha.

## Setup

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

Get the required packages for this project:

```
pip install -r requirements.txt
```

Don't forget you need to add the venv to jupyter in order to run the notebook using your venv.

```
python -m ipykernel install --user --name=.venv --display-name "Python (myvenv)"
```

Select your '.venv' by clicking on 'kernels' and typing in the path or otherwise selecting it. You may or may not need to give visual studio a kick up the bum to get it to work by restarting vsCode.

If you've got it working, you should see this: ![newplot](https://github.com/user-attachments/assets/a0adcabf-1ec7-49d8-bd05-7badf4c20741)
