---
layout: post
title: Add Advanced Features to the Blog
---



This post introduces two advanced features already implemented in jekyll framework: DISQUS and Google Analytics.



After reading this, you'll learn about:

* Using DISQUS comment system to interact with your blog readers
* Using Google Analytics to monitor your blog and better understand your visitors



## DISQUS

DISQUS provides your blog with a comment system, and is built inside jekyll. You may notice in `_config.yml` that there's one entry like this:

```
# Enter your Disqus shortname (not your username) to enable commenting on posts
# You can find your shortname on the Settings page of your Disqus account
disqus:
```

This is where you can enable DISQUS in your blog. But first, you need to get your blog a short name.



Go to [DISQUS](https://disqus.com), follow the instructions to sign up and register your blog. The instructions are clear in the website and I won't talk too much about detailed procedures. Just notice that you need to fill your DISQUS **shortname** to `_config.yml`, and finding that can be a bit frustrating. If you get lost in the website's complex system, refer to [this page](https://help.disqus.com/en/articles/1717111-what-s-a-shortname). This official doc instructed you on finding the shortname in detail.



After filling in the shortname to `_config.yml`, DISQUS should be loaded in the posts of your blog. You will be notified by emails when there's a new comment.



If there displays an error saying DISQUS can't be loaded, check whether your blog is properly registered and whether you get the shortname right. Mostly, that's where things go wrong. Check your network connection either, DISQUS can be unstable or unavailable in some regions.



## Google Analytics

Google Analytics is something you will need when wanting to get an overview of your blog's visitors. It's powerful, with many advanced features. Here, we just talk about the basics.



Go to Google Analytics and register your blog (the procedure is somewhat similar to previous one), after that you'll get a *Google Analytics Web Tracking Code*, copy and paste it here in `_config.yml`:

```
# Enter your Google Analytics web tracking code (e.g. UA-2110908-2) to activate tracking
google_analytics:
```

That's all you need to do. Leave behind the JavaScript code Google Analytics told you to put in your blog after successfully registered, jekyll has included that inside.



When done, go to [Google Analytics](https://analytics.google.com), the system may take some time to fetch data. After that, you can analyze your blog data easily.



## Conclusion

With these two systems, your blog now has a place for interaction and a system for statistical analysis, use them wisely.



Also, notice that using these systems means your blog visitors' information will be gathered or analyzed in some ways, so you'd better add a terms & conditions page or privacy policy page to avoid potential legal issues.



This blog together with the previous two ([The Basics of Building a Blog](https://lincoln-zhou.github.io/The-Basics-of-Building-a-Blog/); [Customize the Blog](https://lincoln-zhou.github.io/Customize-the-Blog/)) briefly introduces ways to build a fully functional personal blog, and those should cover most things you need. More advanced instructions may be introduced in future posts.

