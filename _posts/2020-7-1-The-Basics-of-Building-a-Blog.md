In this post, I will briefly introduce ways to bulid a free personal blog using GitHub Pages and jekyll framework.



Follow the steps, and you will:

* Learn the basics about GitHub Pages and jekyll framework
* Have a personal blog hosted on GitHub Pages and be able to access it with your web browser
* Learn how to add new posts to your blog



To follow the steps smoothly, it's suggested that you should be equipped with the following:

* Basic knowlege of GitHub and Markdown (tutorials can be found [here](https://guides.github.com/features/mastering-markdown/))
* A personal GitHub account



## Create the Blog

Shortly speaking, GitHub Pages offers you an environment to host your static website pages, while jekyll helps you handling most technical things and enables you to focus on content of the blog. A combination of the two makes it easy for beginners to build their personal blogs. While it may not be as powerful as blogs based on other  frameworks such as WordPress, it meets the needs of most people.



To get your blog ready, fork [this repository](https://github.com/barryclark/jekyll-now) to your GitHub account, and change your own repository (which you just forked from the URL above) name to this format:

```
yourName.github.io
// yourName is your GitHub account name
```

For example, if my GitHub account name is Lincoln, change the name of repository to `Lincoln.github.io` .



Now, just wait a minute, then open your web browser and go to `yourName.github.io`, you shall see the icon of jekyll and a notice telling that you're up and running.



Till here, a blog with your unique URL has been generated and is accessible online.



## Add New Posts

Most times, you are suggested to write posts using Markdown, which means you can merely focus on writing the post, and jekyll will handle everything else.



While GitHub website has basic ability to write Markdown, I still recommend you to use a editor you like, such as Typora, Visual Studio Code and so on.



I'm not gonna talk about how to write Markdown here, but be advised, in order to make jekyll recognize your post file, there are some unique syntax you should pay attention to in your `.md` file, for example, each new **post** should start with this:

```
---
layout: post
title: yourTitle //title of this post
---
```



Also, bear in mind that **what you see in your editor isn't exactly what you'll see in the rendered webpage**, the UI can be ugly if you write some part of the Markdown file inappropriately. You may need to try a few times before making the post looks exactly what you want.



After finishing the writing work, let's release the post. First, change the Markdown file name to:

```
YYYY-MM-DD-postTitle.md
```

For example, I have a new post called "About This Blog", and I released it on July 1st, 2020, then the file should be renamed into `2020-7-1-About-This-Blog.md`.



Next, upload the file to `yourName.github.io/_posts` on GitHub, commit changes, done.



Now wait a moment, and the post you just upload will be accessible from the index page of your personal blog.



## Conclusion 

This part is the most basic yet most important one to build a personal blog. In the next post, I'll introduce more on customizing your personal blog.
