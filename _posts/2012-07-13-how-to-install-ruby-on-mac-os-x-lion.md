---
layout: post
title: "[Ruby] How to Install Ruby on Mac OS X Lion"
tags: [ruby, mac os x, install, guide, tutorial, programming]
author_name: Mark Miyashita
author_url: http://markmiyashita.com
google_plus: 101180624276428786239
date: 2012-07-13 21:01:00 -8
---

By default, Lion comes prepackaged with Ruby 1.8.7. However, the one problem with this is that 1.8.7 is outdated. At the time of this post, the most recent version is 1.9.3 which is the environment most current apps are being written in. This guide will help you through the process of setting up Ruby 1.9.3 on your Mac OS X Lion machine.

Step 1) Make sure you have a working version of Xcode 4.1 or greater running on your Mac. Versions 3.x.x will not work very well with Ruby and may cause some install problems. You can download the latest version of Xcode free from the App Store.

Step 2) To check that you are running the right version of Xcode, open up Terminal by going to Applications > Utilities > Terminal and typing in:
    
{% highlight bash %}
    /Applications/Xcode.app/Contents/Developer/usr/bin/xcodebuild -version
{% endhighlight %}

It should say something along the lines of "Xcode 4.3.2 Build version 4E2002" spanning two lines. Next we are going to check our version of Git which is automatically installed by Xcode. Type this line into Terminal:

{% highlight bash %}
    git --version
{% endhighlight %}

This step is to verify that you are running at least version 1.7.4.4 of Git. Okay, now we are ready to begin installing <a href="http://beginrescueend.com/">RVM (Ruby Version Manager)</a>

Step 3) In Terminal, type the following (on separate lines):

{% highlight bash %}
    curl -L get.rvm.io | bash -s stable

    source ~/.rvm/scripts/'rvm'

    rvm requirements
{% endhighlight %}

That last line, "rvm requirements" checks the requirements for RVM. Verify that you meet all of these requirements before proceeding.

Step 4) Finally, the command to install Ruby is:

{% highlight bash %}
    rvm install 1.9.3
{% endhighlight %}

After the install is finished, you should be able to load up the interactive Ruby environment by typing "irb" into Terminal.

Congratulations! You now have the Ruby programming language installed on your Mac. Introduction to Ruby articles will be coming soon with tutorials and comprehensive guides to get you started!