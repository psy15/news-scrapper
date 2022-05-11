# news-scrapper

A script to scrap articles from a news website and post it to a Telegram channel using telegram bot API.

## Config

* Set the following env vars:
  * `TARGET_URL` - webpage to scrap
  * `TOKEN` - telegram bot token
  * `CHANNEL` - telegram channel id (the bot has to be added to this channel as an administrator)
  * `GTOKEN` - github access token 
  * `GIST_ID` -  github gist id
  
  
* Run `python app.py`

## Notes

The last posted url is stored in a gist file, the script will read the last posted url from this gist.
the script will skip all the urls that have been posted earlier until this url is found and will update the latest posted to this file.