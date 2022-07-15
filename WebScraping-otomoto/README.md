# Web Scraping OTOMOTO

<sup align = "left"> 
  
   *Status: The project is finished, it is unlikely to be developed*
  
</sup>

<p>

A simple program that I used to look for new offers of a specific car model in the service [OTOMOTO](https://www.otomoto.pl/).

</p>

## List of contents
1. [Project description](#project-description)
3. [Libraries used](#libraries-used)
4. [How to install](#how-to-install)

## Project description
The project was entirely created using Python 3.10.5.
<p></p>

 This program checked all car advertisements in the service and saved to an excel file those that met my criteria. When an advertisement was already saved in a file, it was omitted. This allowed me to save a lot of time, because browsing all the offers every day was tiring.
  <p></p>
  
In addition, when there is a new advertisement for a car that meets the assumed criteria, an SMS notification with a link to the advertisement is immediately sent. [Twilio](https://www.twilio.com/) service was used to send SMS messages. This program can be run manually or using crontab to check for new ads fully automatic.

#### Libraries used
* openpyxl
* requests
* BeautifulSoup
* twilio

## How to install
1. Download `main.py`, `keys.py` and `config.py`.
2. You should create an account on [Twilio](https://www.twilio.com/) or comment 127th line of code so as not to receive SMS notification.
3. Add your account sid, authorization code, phone number and Twilio number in `keys.py`.
4. Run `main.py`.

##
