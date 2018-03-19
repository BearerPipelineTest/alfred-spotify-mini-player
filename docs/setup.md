---
layout: article
permalink: /setup/
title: "Setup"
date: 2015-01-01
modified: 2017-09-11
toc: true
share: false
noindex: false
---

{% include toc.html %}

Setting up the workflow is easy, you just need to follow these steps:-

## Download and install the workflow

* [Download](https://github.com/packal/repository/raw/master/com.vdesabou.spotify.mini.player/spotifyminiplayer.alfredworkflow) the workflow

* Open spotifyminiplayer.alfredworkflow by double-clicking it or dragging it into Alfred.

## Create a Spotify Application

* Create an [Application on Spotify](https://developer.spotify.com/my-applications) (this is for both free and premium users)
    * You can set Application Name and Description to whatever you want
    * ***Redirect URI must be set to*** `http://localhost:15298/callback.php`

**Warning:** Make sure to click 'Save' button once you set the Redirect URI
{: .notice-danger}

<figure>
	<a href="{{ site.url }}/images/setup1.jpg"><img src="{{ site.url }}/images/setup1.jpg"></a>
	<figcaption>Example of Spotify Application (click to enlarge).</figcaption>
</figure>


Note: if you're using a firewall or a software that blocks communication, note that you'll have to unblock the following domains to use the workflow:-

* https://api.spotify.com (for interaction with Spotify)

* https://raw.githubusercontent.com (for downloading new release from Packal)

* https://github.com/ (for downloading images when changing theme)

* http://api.stathat.com (for statistics)

* https://transfer.sh (for DEBUG Zip file)


Also, if you're using a proxy, don't forget to enable this option in Alfred preferences:-

<figure>
	<a href="{{ site.url }}/images/setup6.jpg"><img src="{{ site.url }}/images/setup6.jpg"></a>
	<figcaption>Use Mac OS http proxy settings for scripts option.</figcaption>
</figure>


## Create the library

**Warning:** If you use a proxy, make sure to activate **Use macOS http proxy settings for scripts** in Advanced tab of Alfred Settings
{: .notice-danger}

* Invoke the workflow (with keyword `spot_mini`, or with an [hotkey]({{ site.url }}/articles/hotkeys) ) 

* Follow the steps as below by copy/pasting the Client ID and Client Secret into Alfred window when asked:

<figure>
	<a href="{{ site.url }}/images/setup.gif"><img src="{{ site.url }}/images/setup.gif"></a>
	<figcaption>Paste Client ID and Client Secret (click to enlarge).</figcaption>
</figure>


* Invoke the workflow again and select Authenticate with Spotify, your web browser will open and you'll be prompted to login with Spotify and allow access to your application.
At the end you should see a message like this:-

>Hello <your name here> ! You are now successfully logged and you can close this window.

* Invoke the workflow again and Create the library.

* You can check progress by invoking the workflow again:-

<figure>
	<img src="{{ site.url }}/images/setup2.jpg">
	<figcaption>See progress by invoking workflow.</figcaption>
</figure>


* After some time, you should get a notification saying that library has been created.

<figure>
	<img src="{{ site.url }}/images/setup3.jpg">
	<figcaption>Library created (43 seconds for 2500 tracks).</figcaption>
</figure>

* Then you can use and enjoy the workflow. The artworks are downloaded in the background, you should get a notification when background download starts:-

<figure>
	<img src="{{ site.url }}/images/setup4.jpg">
	<figcaption>Notification for the start of background download of artworks.</figcaption>
</figure>

* During that time, you can use the workflow (you'll see the progress at the top of main menu), and you can see some blank artworks:-

<figure>
	<img src="{{ site.url }}/images/setup5.jpg">
	<figcaption>Example of blank artworks until the end of background download is over.</figcaption>
</figure>



