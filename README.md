# FakeNewsify

This project was done for the Same Home Different Hacks Hackathon. The competition's main theme was using their tools such as GCP, MongoDB, UI, and Domain.com to build something benificial to people stuck at home during quarantine. Due to the recent situation with a lot of news coverage, we decided to create a web app that can help detect which of these news articles are real and authentic and which of them are fake. These will also better help users decipher between which sources to follow and which to take in through one ear, and out the other. 

A link to our devpost submission can be found here: https://devpost.com/software/fakenewsify-news-credibility-checker

A link to a small YouTube demo can be found here: https://www.youtube.com/watch?v=rbDgyr0pr6o

The app is currently deployed to heroku, you can check it out here: https://fakenewsify.herokuapp.com/

## Screenshots Of Core Pages 

Our web app comrises of 4 different views. The home view allows users to enter article url links directly and get immediate results on the title and summary of that article as well as whether or not it's real/fake or clickbait/not clickbait. The about page summarizes the apps intention and main functions. The live feed page is where our app gets data from the Python news api and constantly updates the page with new news articles as well as an image of their thumbnail, their url, headline, and whether or not they're real/fake or clickbait/non clickbait. Our final page trends is where we use our user submitted data combined with MongoDB to create these google analytics charts to compare fake vs real sources and clickbait vs non clickbait ones. 

These are pictures of some of our main pages.

### Our Home Screen 

![](img1.PNG)

### Dark Mode On All Pages For Accessibility

![](img2.PNG)

### About Page

![](img4.PNG)

### Dark Mode For Accessibility

![](img5.PNG)

### Live Feed Page

![](img3.PNG)

## Features

* NLTK article summarization
* NLTK article clickbait vs non clickbait recognition
* Machine learning fake vs real article recognition
* Dark mode on all pages
* Live feed of news articles connected with Python news API
* Live graphs connected to MongoDB to analyze articles

## How We Built It

We built the back-end infrastructure of our app with Flask, this allows us to do multi-page rendering as well as parsing variables and values to HTML templates and write Python within these templates. We're using NLTK, Scikit-Learn, Pandas, and Numpy to compile data and create our machine learning models. We're using the newsapi to collect data from news articles being updated constantly. We're then using a MongoDB database along with Googles chart drawing features to create nice graphics to provide visuals on these different news article statistics.

## Clone

```
git clone https://github.com/aahmad4/FakeNewsify-Article-Credibility-Checker
```

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the required packages.

```bash
pip install -r requirements.txt
```

## Usage

First make sure you download NLTK properly
```
python
>>> import nltk
>>> nltk.download()
```
Run app.py
```
python app.py
```
Then go to 
```
http://127.0.0.1:5000/
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
