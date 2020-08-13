<p align="center">
  <img src="readme/coollogo.gif">
</p>

<p align="center">
    <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/thaniel-c/summer-code-jam-2020">
    <img alt="GitHub" src="https://img.shields.io/github/license/thaniel-c/summer-code-jam-2020?color=%23009dff%20">
    <a href="https://discord.gg/python">
        <img src="https://img.shields.io/static/v1?label=Python%20Discord&logo=discord&message=%3E80k%20members&color=%237289DA&logoColor=white">
    </a>
</p>

Blast off to the past and surf the web 90s style! With SpydirWeb, you can browse a your own private version of the early internet! Get lost in hundreds of webpages, all generated with AI text generation, webscraping, and other methods to bring you an immersive experience! 

# Table of Contents
  * [Overview](#overview)
  * [Installation](#installation)
  * [License](#license)
  * [Authors](#Authors)

# Overview

**SpydirWeb** has three different types of pages: Information, Blogs, and Business. The blog and business pages use [OpenAi's gpt-2](https://github.com/openai/gpt-2) AI to generate the content, while the info pages use the [Wikipedia](https://pypi.org/project/wikipedia/) package. Images are retrieved using the [Pixabay API](https://pixabay.com/api/docs/).

Click one of the three links listed on the home page to get started browsing Spydirweb.

![](readme/home.png)

Click any link on the page to browse further.

![](readme/info.png)

The text in the blog and business pages may take a while to load, as they are generated with an AI.

![](readme/blog.png)

That's it! Have fun browsing!

![](readme/blogdone.png)
 
# Installation

Before we start, make sure you have at least 1 GB of free space.

#### Code Jam Judges Only:
Please check the `#talented-tigers` channel on the discord server. Copy and paste the text block we sent into a file called `.env` in the `talented-tigers` directory.

#### Non-Code-Jam-Judges Only:
You will need your own API key for Pixabay, which SpydirWeb use for collecting images. Go to [Pixabay's website](https://pixabay.com/api/docs/) to get a key and then make a new file called `.env` with:
```
API_KEY=your_key_here
```
written inside of it (replace `your_key_here` with your API key)

#### Requirements (All):
  * [Git](https://git-scm.com/)
  * [Python 3](https://python.org) (Make sure it is added to your system's path)

#### Setup (Windows):
  * Install [Docker for Windows](https://docs.docker.com/docker-for-windows) (or [Docker for Windows 10 *Home*](https://docs.docker.com/docker-for-windows/install-windows-home/)).
  * Install pipenv with `pip install pipenv`
  * Open a powershell window and clone the repository by running `git clone https://github.com/thaniel-c/summer-code-jam-2020.git`
  * Then run these following commands:
    * `cd summer-code-jam-2020/talented-tigers`
    * `pipenv run python run-windows.py`
  * The last command will run the website locally, you will be able to view the website at the address `localhost:8000`.

#### Setup (Linux):
  * Install [Docker](https://docs.docker.com/engine/install/) (Or for Arch - [Docker on Arch](https://www.google.com/search?client=firefox-b-1-d&q=docker+arch))
  * Clone the repository by running `git clone https://github.com/thaniel-c/summer-code-jam-2020.git`
  * Next install `pipenv` by running `pip3 install pipenv` (may require `sudo` if it isn't automatically added to path, you can test it with `pipenv --version`. Also make sure pip is installed: https://pip.pypa.io/en/stable/installing/)
  * *If* `pipenv` can not automatically detect your system's path to Python, you may need to run `pipenv --python /path/to/python` to tell `pipenv` the path to Python.
  * Then run these following commands:
    * `cd summer-code-jam-2020/talented-tigers`
    * `pipenv run python3 run-linux.py`
  * The last command will run the website locally, you will be able to view the website at the address `localhost:8000`.

#### Alternative Installation
Alternatively, you can run each command in the run scripts one by one, the run scripts only exist to better hide the API key and make the setup process shorter. These are the commands:

#### Windows commands:
  * `docker build -t spydirweb -f Dockerfile .`
  * `docker run -e <API KEY> -it -p 8000:8000 spydirweb`

#### Linux commands:
  * `sudo docker build -t spydirweb -f Dockerfile .`
  * `sudo docker run -e <API KEY> -it -p 8000:8000 spydirweb`

If you decide to run the site this way, replace `<API KEY>` with your Pixabay API key. The `.env` file is **not** needed.


Installation and loading can take a while as we need to setup the models for the AI as well as the dictionary for the link parser. Hang in there!

**Note**: Be sure to view the site at http://localhost:8000, other hosts may not work as expected.

# License
```
MIT License

Copyright (c) 2020 Python Discord

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
# Authors
Team Talented Tigers is..
* **Nathan Coulas (GitHub: [thaniel-c](https://github.com/thaniel-c), Discord: [thaniel#3631](https://discordapp.com/channels/@me/703922100112457778/))**
* **Sloopoo (GitHub: [flextian](https://github.com/flextian))**
* **Garfellow (GitHub: [Garfellow](https://github.com/GarfellowGMOD))**
* **SuperMaZingCoder (GitHub: [CodeForeverAndEver](https://github.com/CodeForeverAndEver))**
* **Ice Wolfy (GitHub: [Icebluewolf](https://github.com/Icebluewolf))**

<p align="center">
<a href="#" >
    <img src="readme/banner.png" alt="LogoMakr_5RDTOc" width=100%>
</a>
</p>

<sub>
<p align="center">
(Talented Tigers logo made by neon#9865, a helper on the <a href="https://pythondiscord.com/">Python Discord</a> </a> using <a href="https://logomakrcom">logomakr</a>)
</p></sub>
