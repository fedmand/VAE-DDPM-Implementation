# Deep Learning Coursework 2: Generative models

The notebook dl_cw2.ipynb provides the skeleton for Coursework 3, focusing on generative models (VAEs and Diffusion models).
Setup instructions, depdency requirements, and running instructions are provided in the same notebook.
For any questions, please post a message on EdStem. Good luck!

## Local testing

This notebook contains two public tests and one private test (VAE parameter size and DDPM schedules). You should be able to run the public tests locally by running the first notebook cell which is the otter setup.

## GPUDojo setup

For this coursework, we recommend working with GPUDojo, although imperial resources are also accessible.

### Requesting an instance

To connect to a GPUDojo instance, simply visit [gpudojo.doc.ic.ac.uk](gpudojo.doc.ic.ac.uk).

Once the instance has been created, simply click "Open Jupyter on your VM". You can also connect remotely via ssh and work with VS Code. Intructions on this setup will be available on an EdStem announcement shortly.

### Cloning repository and setting up an environment

Open a Terminal, clone the CW2 repository, and cd into it:

``git clone https://gitlab.doc.ic.ac.uk/lab2526_spring/<cohort-code>_DL_CW_2_<user-id>.git``

``cd <cohort-code>_DL_CW_2_<user-id>``

Now we need to create an environment to install our packages. Let's install pipenv and create it:

``sudo apt install pipenv``

``pipenv install``

Now that we have our environment installed, let's activate it in our Terminal and installed the required dependencies.

``pipenv shell``

You should see here the name of your environment in parentheses `(<cohort-code>_DL_CW_2_<user-id>)`.

``pip install -r requirements.txt``

This should run and install all your dependencies. Your setup is almost ready. Make sure your kernel is visible by jupyter notebook!

### Syncinc environment to notebook kernels

It might happen that when opening the notebook, your python kernel is not visible. This is because your notebook cannot find your environment path. Let's fix this! Run the following commands on a terminal (inside your CW2 repository).

``pipenv shell``

``pip install ipykernel``

``python -m ipykernel install --user --display-name "Python (dl_cw2)"``

Now when opening your notebook, you should see a kernel available named `Python (dl_cw2)`.
