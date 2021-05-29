# Create python virtual environment on Window


### Create a new virtual environment by choosing a Python interpreter and making a .\venv directory to hold it:

```bash
python -m venv --system-site-packages .\keras-venv
```



### Activate the virtual environment:

```bash
.\keras-venv\Scripts\activate
```



### Install packages within a virtual environment without affecting the host system setup. Start by upgrading pip :

```bash
pip install --upgrade pip
pip list  # show packages installed within the virtual environment
```



### And to exit the virtual environment later:

```bash
deactivate  # don't exit until you're done using TensorFlow
```