# #2 Tech Knowledge Drop - How to running code every day for free

Hi guys, this week my friend Halmenschlager went to me asking for help he had a demand to develop

I want to call the Steam API endpoint to clear every single day the leaderboard of a game that we have. I don't want to create a server for that and mainly it needs to be 0 cost.

Understanding his use case I started explain to him what he needs for accomplish this challenge.

1. He needs to understand the options that he has to run scripts without a server, in this case locally or in cloud.
2. He needs a something for scheduling tasks.


## How to run locally scripts without a server?

Well, we can easily run a script locally in our machine, any programming language can call apis without the need of running a server.

To run every day in a week, he could use a cron job triggering the script without any hands.

Simple way to create a cron, open the terminal and run this command:

```sh
crontab -e
```

And add your schedulers like this one that runs at 04:00 a.m. every day. See more [here](https://crontab.guru/#5_4_*_*_1).

```sh
0 4 * * 0-6 /home/ramon/script.sh > /dev/null 2>&1
```

But nothing is so simple in this life, he needs for his work he can't run everything in his machine.

It's not secure and it's not scalable, because if someone of the company needs to maintain that script, or make it up they will not have access.

So we need a solution that everyone in the team can access that scheduled script.

## How to run scripts without a server in cloud?

First we need to choose our cloud provider, the big players are AWS, Microsoft Azure, and Google Cloud.

For this article we will use AWS services like Amazon EventBridge Scheduler, and Lambda functions.

That's all folks!

Feel free to comment, share it with your friends, and like it!

### References so you can study: 
https://phoenixnap.com/kb/set-up-cron-job-linux