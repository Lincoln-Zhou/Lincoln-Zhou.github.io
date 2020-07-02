---
layout: post
title: Customize the Blog
---

This post introduces how to make the blog looks more decent.



After reading this, you will learn how to:

* Customize your blog's name and description shown in web browser
* Add personal contact information to your blog
* Use images in your blog
* Add a favicon to your blog
* Add a new page to your blog



## Customize with the _config.yml

In the root directory of your GitHub Pages project, you should find the `_config.yml`   file. This is where you control website properties in jekyll, and is exactly what we need to complete the first two tasks.



The file has detailed instructions inside, informing you about what and how to change. Currently, don't mess with anything else, just go to the `name` and `description` entry to customize your name and the blog's description.



To add your personal contact information, go to the `footer-links` part, and choose entries you want to add. For example, if you want to publish your GitHub account info, fill that entry with your GitHub account name, and an icon will appear at the bottom of your blog linking to your GitHub account's profile page. Use this wisely, bear in mind that anyone can see it, so make sure you only publish profiles links to those you feel free to make public.



In later blog posts I will introduce more about using `_config.yml`, right now we have all we need. Remember to commit file changes to your repository before closing the tab.



## Use Images In the Blog

Images help making the blog looks better. In your blog, you're supposed to store most images used in the `/images` directory. To use the image uploaded to GitHub, open the image, right click on the previewed image and choose `Open Image in New Tab` (if no preview options available, choose `View raw`), then copy the new tab's URL. Under most circumstances, the URL will be something like:

```
https://raw.githubusercontent.com/userName/userName.github.io/...
```

Then you can use this URL in your post's `.md` file to show an image or to config your avatar in `_config.yml`. 



Be advised, this is only one of the solutions, you actually can upload the image file to wherever you prefer, just make sure the image is accessible in the public Internet. For example, upload the image to some host provider such as [Imgur](https://imgur.com/) and use the generated link in your blog also works, while upload to your personal Google Photos may fail, since it can be accessed only with your personal Google account.



## Add a Favicon

To add a favicon, you need to have some favicon icons first. You can design one by yourself (which can be unique but time-consuming), or just use some online generators, such as [favicon.io](https://favicon.io/favicon-generator/).



Now you have a favicon file named `favicon.ico`, upload it to root directory of your blog repository in GitHub.



Next, go to `/_layouts/default.html`, in the `head` part of the file, add the following code:

```html
<link rel="shortcut icon" type="image/x-icon" href="/favicon.ico?">
```



Commit changes and wait a minute, your blog should have a customized favicon now, no more being ugly with Google Chrome's default favicon.



## Add a New Page

Sometimes we want something more than merely posts in the blog. For example, adding a privacy policy page. This isn't complex. You can write the content of this new page in Markdown and let jekyll render it for you, the front matter is a bit different. To create a new **page**, add something like this in the beginning of your `.md` file:

```
---
layout: page
title: Privacy Policy
permalink: /privacy.html
---
```

Next, rename the file to something like `privacy.md`, and upload it to the root directory of the repository. 



Now, your new page can be accessed with `https://yourBlogName/privacy.html`.



Please notice, you can also create more organized pages using subfolders, the official docs can be found [here](https://jekyllrb.com/docs/pages/).



## Conclusion

This part can be a bit complex sometimes, and a few glitches may happen. Remember to refer to the official docs when encountering problems. In the next post, I'll introduce ways to monitor your blog and interact with readers better, using Google Analytics and DISQUS.
