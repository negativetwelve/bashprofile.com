---
layout: post
title: "How to Change Directories"
tags: [Unix, Tutorials]
author_name: Mark Miyashita
author_url: http://markmiyashita.com
google_plus: 101180624276428786239
date: 2012-07-13 21:15:00 -8
image: terminal.png

category: Unix
featured: true
feature-number: 0
---

<img class="post-image" src="{{site.url}}/images/terminal.png" title="Terminal">

In Unix or any sort of Terminal interface the quickest way to navigate through folders is to use the <code>cd</code> command. You simply type:

{% highlight bash %}
    cd 'folder_name'
{% endhighlight %}

to change the directory into the folder name. A simple shortcut to change into the directory one level up is to type in:

{% highlight bash %}
    cd ..
{% endhighlight %}

In Unix, one dot "." resembles the current directory, while two dots ".." signifies one directory up. To reiterate, if my folder structure was:

{% highlight bash %}
    ~/folder/sample/structure/files
{% endhighlight %}

and I was in the "sample" folder, to get to the folder called "folder" I would simply just type:

{% highlight bash %}
    cd ..
{% endhighlight %}

To get to the folder labeled "structure" I would type:

{% highlight bash %}
    cd structure
{% endhighlight %}

It is that simple!
Hope this hint helped you! Please post in the comments below with suggestions of future articles and questions, thank you!