## Linky

Project is built with flask, requests, and beautifulsoup

#### 2 components:
  1. web app
  2. web crawler

#### Web App
The database search just checks if any of the words you enter are in any of the
words in the _title_ all the websites in the database

The websites are not ranked.

front-end: html, css
back-end: sqlite3, flask

#### Crawler
Obtains website links and stores in database

The crawler needs a seed website to start crawling from and can be started like
so:

`flask crawl seed`

example:

`flask crawl http://coinmarketcap.com/bitcoin`

The crawler stores only two items:
link: http link address
title: whatever is in the <title> tag

Uses requests to get webpages and beautifulsoup to extract links and titles
