# #1 Tech Knowledge Drop - Why I decided to use NoSQL

Hi guys, this is my first drop of knowledge that I want to share with you!

Nowadays we don't want to read a lot to only consume some insights of knowledge. We want to gain insights, process a little, save them in our brain cache, and then, when needed, recover that insight and dive deeper into research for more content, books, articles, etc.

In summary, this project is about sharing insights and knowledge focused on answering simple and direct questions created by myself, friends, or the community.


## Why I've chosen NoSQL DB for this project?

I'm working on a personal project that will crawl the internet looking for new artists and their concerts schedules every day.

This crawler's use case will produce a tons of data every day, so I started asking myself what type of database I should use. 

In answering this question, I decided to use a NoSQL DB. 

### Some reasons:
- **Flexible schemas:** I will probably need to save unstructured data depending on my concert sources.
- **Fast queries due to the data model:** The application will need to have a robust search engine so users can easily and quickly find artists and their concerts.
- **Data type is friendly:** The project will be developed in Javascript, and a NoSQL DB can easily retrieve data in JSON format.

That's all folks!

Feel free to comment, share it with your friends, and like it!

### References so you can study: 
https://www.mongodb.com/nosql-explained
https://www.mongodb.com/basics/full-text-search
https://www.mongodb.com/docs/manual/data-modeling/#flexible-schema
