<div id="top"></div>

<!-- PROJECT LOGO -->
<br>
<div align="center">

  <h3 align="center">ScoopIt Bot</h3>

  <p align="center">
    Project of the bot to the Instagram which enables follow for follow actions.  
    <br>
    <br>
    <a href="http://www.youtube.com/watch?feature=player_embedded&v=Dt9_tAM2ofQ" target="_blank">
	    <img src="http://img.youtube.com/vi/Dt9_tAM2ofQ/0.jpg" alt="YouTUbe video" width="240" height="180" border="0"/>
    </a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

A project meant for automatically create post on scoopIt platform.

Here's why:

- Have to add posts each day at morning and evening at the same hour
- Have to add posts for 15 days straight
- Just too lazy to do it by myself
- Want to do something different meanwhile adding post
- Create enough save app with login process
- Publish app

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

Include all components used in the project.

- [Python 3](https://www.python.org/)
  - [Selenium](https://selenium-python.readthedocs.io/)
  - [Time](https://docs.python.org/3/library/time.html)
  - [Pyperclip](https://pypi.org/project/pyperclip/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->

## Getting Started

Instructions on setting up project locally. To get a local copy up and running follow these steps.

### Prerequisites

<div id="prerequisites"></div>

Things you need to use for the software and how to install them.

1. Open chrome browser

- Go to the settings -> About Chrome
- Check chrome driver version (_in my case 100.0.4896.127_)
  <img src=".\img to README\chrome version.jpg">

2. Download Chrome driver matching your version

- <a href="https://chromedriver.chromium.org/downloads">Link to download driver</a>
- Choose link to download page, based on your first number of version (_in my case 100.x.x.x_)
- Choose your sysyem version and download driver (_in my case chromedriver_win32.zip_)
  <img src=".\img to README\chromedriver download.jpg">

3. Extract files, and copy chrome driver to directory named driver of the project

4. Instal Selenium and Pyperclip module (_cmd_)
   ```sh
   pip install selenium
   pip install pyperclip
   ```

### Installation

_Installing and setting up app._

1. Clone the repository
   ```sh
   git clone https://github.com/filipwroblewski/ScoopIt-bot
   ```
2. Install required modules
   ```sh
   pip install selenium
   pip install pyperclip
   ```
3. Check your Chrome diver version and if it is different than used in the project repeat process in <a href="#prerequisites">Prerequisites (1, 2, 3)</a>

   <p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->

## Usage

1. Structure of <em>data.txt</em> file.

   - First line: <b>login name</b>
   - Second line: <b>link to the article about your post</b>
   - Third line to the end of file: <b>content about the post</b>

2. Copy (_Ctrl + C_) password to your account to clipboard.

3. Run _scoopIt bot.py_.

   ```sh
   python "scoopIt bot.py"
   ```

Program automatically locate elements on the site based on the HTML code using xpath and ids. App insert data given in the _data.txt_ file and data from clipboard.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ROADMAP -->

## Roadmap

- [x] Contains data
  - [x] Data in the \*.txt file
    - [x] Login name
    - [x] Link to the artile
    - [x] Content of the post
      - [x] Enable multiline text
    - [x] Use utf8 encoding to use all characters
  - [x] Password
    - [x] Make password save
      - [x] Contains password in pyperclip
      - [x] Reset pyperclip after collect password
- [x] Create object of ScoopIt user
  - [x] Nick
  - [x] Password
  - [x] Run chrome driver
- [x] ScoopIt user login
  - [x] Automatically open browser
    - [x] Enable to take actions in browser
  - [x] Open scoopIt website
  - [x] Login to scoopIt
    - [x] Locate login field
      - [x] Insert login name
    - [x] Locate password field
      - [x] Insert password
    - [x] Log in
- [x] Add post to ScoopIt
  - [x] Locate add new post button
  - [x] Insert link to the article
  - [x] Insert data about description of the article
- [x] Publish app
- [ ] Create time schedule to run App automatically

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->

## License

<!-- Distributed under the ________ License. See `LICENSE.txt` for more information. -->

Distributed without any License yet.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->

## Contact

<a href="https://twitter.com/wrobl_ewski" ><img src="https://img.shields.io/twitter/follow/wrobl_ewski.svg?style=social"></a>

<p align="right">(<a href="#top">back to top</a>)</p>
