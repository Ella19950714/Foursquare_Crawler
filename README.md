
# foursquare_crawler
This crawler is designed to collect information from Foursquare website(www.foursquare.com ).</br>Using Foursquare API.</br> 
# System Requirements
Ubuntu (Version: 14.04). This project haven’t been tested on other platform.
# Pre-request Packages
This crawler is written in Python 2.7.11
Other pre-request packages include:
Httplib2(https://pypi.python.org/pypi/httplib2 )
Guess language 0.2(https://pypi.python.org/pypi/guess-language )
* You can run install.sh to install them.    
# Output Format
   This crawler returns a json format profile.</br>
   example format:</br>
   
    {   
           "user info": {     
           "country": "US",      
           "address": "New York, NY",     
           "user id": "32",      
           "exist": (_1 for yes 0 for no_),      
           "gender": "m"(_m for male and f for female_),     
           "imgURL": xxxx(_user icon url_)
           },        
           "tips": {     
               "count": 647(_total number of tips_),     
               "tips content": [     
                   { 
                       "category": "Food",     
                       "polarity": 0.049(_sentiment test score_),      
                       "timespam": "1450378655",      
                       "text": "xxxxx",      
                       "len": 148(_length of the text_),      
                       "photo": "y ",      
                       "venue name": "Mimi Cheng's"     
                    }, 
                    ..._other tips_... 
                ] 
    } 
    
# Usage
   Run foursq_crawler.py 
   You may change the start point, finish point (the user ID that the crawler begins and ends) and step (the interval).
