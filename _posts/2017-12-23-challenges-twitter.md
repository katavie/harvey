---
title: The Challenges of Collecting Twitter Data
date: 2017-12-23
---

## The Challenges of Collecting Twitter Data

Every minute, an average of 350,000 tweets are posted on Twitter. Extracting this data is a challenge because Twitter's free APIs, including Search and Streaming, only provide access to a limited selection of content. The Streaming API, for instance, is intended for real-time or current analysis, and users can only query tweets less than 7 days old.

To download the full "firehose" or complete historical records of tweets, one must pay for an enterprise-level API or third-party service.

Twitter's free Streaming API only allows access to the past week of tweets, but Hurricane Harvey occurred several months ago. There are a handful of datasets of Harvey tweets available online, but I'd like to have control over the parameters I use.

To deal with this issue, I used [Twitterscraper](https://github.com/taspinar/twitterscraper), an open-source command line client that "scrapes" search results. While it eliminates the limitation of content having to be less than a week old, it does rely on a search algorithm. I made a word cloud of frequent terms in the dataset I obtained:

![Word cloud of terms from Harvey tweets]({{'/img/wordcloud.jpg'|prepend:site.baseurl}})

Looks like everything on Twitter that was Harvey-related is about weather, right?

Well, we know that Twitter is home to millions of other topics. Even within Harvey-related posts, I would expect posts expressing sympathy, need for help, messages to friends and family, and more.

So this is a challenge that I have yet to fully resolve. If I had more time, I would research more deeply into other options, but I think I'll focus on working with this dataset for now, and revising my background section.