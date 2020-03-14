# HW4 - Continued
**I had my HW4 continued part done on time in my [HW4 repo](https://github.com/BUEC500C1/video-JWangNov). 
This is only the copy of HW4 web service working part.**

## Flask Setup
(quite ez...)

```
virtualenv venv

source venv/bin/activate
pip install -r requirements.txt
pip install flask python-dotenv flask-wtf

flask run -h 0.0.0.0 -p 8421
```

## Web Service Introduction
The web service collects the most recent 10 tweets of an account, converting them to a short video clip.

I run the Flask server on my AWS (*3.136.158.120:8421*). While the server is running, you can easily access the [web page](http://3.136.158.120:8421/).

There will be 5 links of videos. Click anyone of them and you will start downloading a video of the most recent 10 tweets of that account.

Or, use command line to download can also be a good way.

```
curl http://3.136.158.120:8421/lagav -o ./Lagavulin_is_the_best_whisky.mp4
curl http://3.136.158.120:8421/laphr -o ./Laphroaig_is_2nd_best_whisky.mp4
curl http://3.136.158.120:8421/klcho -o ./Kilchoman_impressive_new_distillery.mp4
curl http://3.136.158.120:8421/bnrmc -o ./Benromach_use_nice_beer_yeast.mp4
curl http://3.136.158.120:8421/cdsde -o ./Clydeside_has_NO_TASTE.mp4
```

Please contact me to get access to this web service.
