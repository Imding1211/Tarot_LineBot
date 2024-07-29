<a id="readme-top"></a>
# Tarot_LineBot


<ol>
  <li><a href="#about-the-project">About The Project</a></li>
  <li><a href="#built-with">Built With</a></li>
  <li><a href="#getting-started">Getting Started</a></li>
  <li><a href="#contact">Contact</a></li>
</ol>

## About The Project

This project is a Line Bot designed for tarot card drawing. Users can interact with the bot to receive tarot card draws directly through the Line messaging app.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Built With

* Flask
* line-bot-sdk
  
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

To get a local copy up and running, follow these simple steps.

1. Create a new conda environment
   ```sh
   conda create --name Tarot_LineBot python=3.11
   ```
   
2. Activate environment
   ```sh
   conda activate Tarot_LineBot
   ```

3. Clone the repo
   ```sh
   git clone https://github.com/Imding1211/Tarot_LineBot.git
   ```
   
4. Change directory
   ```sh
   cd Tarot_LineBot
   ```
   
5. Install the required Python packages
   ```sh
   pip install -r requirements.txt
   ```

6. Add your Line token and secret to the token and secret variables in main.py.
   ```sh
   token = 'your Line token'
   secret = 'your Line secret'
   ```
   
7. Install Ngrok

   [Download Ngrok](https://ngrok.com/download)

8. Activate Flask
   ```sh
   nohup python main.py > Tarot_LineBot.log 2>&1 &
   ```

9. Activate Ngrok
   ```sh
   nohup ngrok http http://localhost:8080 > Tarot_LineBot_ngrok.log 2>&1 &
   ```
   
10. Get your API URL.
    ```sh
    wget http://127.0.0.1:4040/api/tunnels
    cat tunnels
    ```

    Find "public_url," which is your API URL.

11. Paste your URL into your Line Developer Webhook URL.
    ```sh
    Your URL/callback
    ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

Chi Heng Ting - a0986772199@gmail.com

Project Link - https://github.com/Imding1211/Tarot_LineBot

<p align="right">(<a href="#readme-top">back to top</a>)</p>
