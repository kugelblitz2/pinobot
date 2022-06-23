# pinobot
A bot to remind Daniel to stop committing during work hours

## How To Use
Configure `settings.py`, cd into the directory and run

    pip3 install -r requirements

to install dependencies. Then,

    python3 bot.py

to start pinobot.

## Running as a service
Change the path in `pinobot.service` to the location of your `bot.py` file

    sudo pip3 install -r requirements
    sudo cp ./pinobot.service /etc/systemd/system
    sudo systemctl daemon-reload
    sudo systemctl enable pinobot
    sudo systemctl start pinobot


**Compatibility Notice: Runs on all real (UNIX) operating systems. May or may not work on Windows**
