# Ubuntu Sheet
A list of command use on Ubuntu
<br/><br/>


### Install Git on Ubuntu 20.04

```bash
sudo apt update             ;\
sudo apt install git -y     # Install Git with Default Packages
git --version               # Check Git version
```

### Prepare environment for deep learning

#### 1. Install Python 3 and Set Up a Programming Environment

- Ubuntu 20.04 and other versions of Debian Linux ship with Python 3 pre-installed. To make sure that our versions are up-to-date, let’s update and upgrade the system with the apt command to work with Ubuntu’s **A**dvanced **P**ackaging **T**ool:

  ```bash
  sudo apt update             ;\
  sudo apt -y upgrade         ;\
  python3 -V                  # Check Python version
  ```
  
- Install **pip**

  ```bash
  sudo apt install -y python3-pip
  ```
  
#### 2. Setting Up a Python Virtual Environment

- Let’s install **venv** by typing:

  ```bash
  sudo apt install -y python3-venv
  ```

- Go to the directory where you would like the environments to live, you can create an environment by running the following command

  ```bash
  python3 -m venv {enviroment_name}
  ```
- Essentially, pyvenv sets up a new directory that contains a few items which we can view with the ls command:

  ```bash
  ls {enviroment_name}
  ```
  
  ```bash
  **Output**
  
  bin include lib lib64 pyvenv.cfg share
  ```
  
- To use this environment, you need to activate it, which you can achieve by typing the following command that calls the **activate** script:
  
  ```bash
  source {enviroment_name}/bin/activate

  ```



### Reference
- [Lisa Tagliaferri, (2020, May 29), How To Install Git on Ubuntu 20.04](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-20-04)
- [Lisa Tagliaferri, (2020, April 24), How To Install Python 3 and Set Up a Programming Environment on an Ubuntu 20.04 Server](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server)
