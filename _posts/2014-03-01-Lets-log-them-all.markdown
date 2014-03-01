---
title: Let's log them all!
layout: post
date:   2014-03-01 12:00:00
categories: logs
---

Since the beginning of Mailee.me we didn’t care too much about the logs. Like everything is being logged but rarely we read it. The only case we really check it was doing a deep investigation about a bug or something like it.

But recently I started to see interesting use cases for log analysis. In our case it would be pretty useful for our support team to check all the steps of an user, so they can understand all the scenario and provide a better experience to the final user.

Also if you want to scale your application to services like Heroku or Amazon OpsWorks you would need a central syslog server. Probably as things start to grow reading log files should become a huge mess.

The initial idea was to signup for a SAAS platform to make all this things. It’s not expensive. And deploying all the infrastructure to the backend of this kind of solution can be painful.

First I took a look at the commercial solutions. Everybody says Splunk is the best one, but their enterprise prices makes it hard for startups. They offer a SAAS version called Splunk Storm that’s free for less than 500MB of logs per month. Also there is logentries.com (that looks very interesting) and also loggly.com.

The point is that my hacker ego won’t let me give up before trying :)

So I started to study the open source solutions and discover a really nice trio: Elastic Search + Logstash + Kibana (check out the final result at <a href="http://demo.kibana.org" target="_blank">demo.kibana.org</a>). I can’t say it’s simple to deploy, but after studying it a little bit, it took me 2 days to make it work, I’ll show you how in the next posts.


