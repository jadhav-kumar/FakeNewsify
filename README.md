# FakeNewsify

This project was done for the Same Home Different Hacks Hackathon. The competition's main theme was using their tools such as GCP, MongoDB, UI, and Domain.com to build something benificial to people stuck at home during quarantine. Due to the recent situation with a lot of news coverage, we decided to create a web app that can help detect which of these news articles are real and authentic and which of them are fake. These will also better help users decipher between which sources to follow and which to take in through one ear, and out the other. 

A link to our devpost submission can be found here: https://devpost.com/software/fakenewsify-news-credibility-checker

## Screenshots Of Core Pages 

Our web app comrises of 4 different views. The home view allows users to enter article url links directly and get immediate results on the title and summary of that article as well as whether or not it's real/fake or clickbait/not clickbait. The about page summarizes the apps intention and main functions. The live feed page is where our app gets data from the Python news api and constantly updates the page with new news articles as well as an image of their thumbnail, their url, headline, and whether or not they're real/fake or clickbait/non clickbait. Our final page trends is where we use our user submitted data combined with MongoDB to create these google analytics charts to compare fake vs real sources and clickbait vs non clickbait ones. 

### Our Home Screen 

![](img1.PNG)

### Dark Mode On All Pages For Accessibility

![](img2.PNG)

### Live Feed Page

![](img3.PNG)
