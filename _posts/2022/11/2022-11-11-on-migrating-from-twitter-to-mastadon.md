---
title: On Migrating From Twitter To Mastodon
categories:
- Geek
tags:
- mastadon
- twitter
- geek
---
When I last wrote about Mastodon [almost three years ago]({{ "/2019/12/16/how-to-post-instagram-posts-on-mastodon-using-ifttt.html" | relative_url }}), I was tinkering about with what was then a niche Twitter alternative, with a small but devoted, mainly tech based, userbase.

However, that's all changed now. Since Elon Musk's buyout of Twitter has amplified existing problems on the platform, and added [financial](https://www.theverge.com/2022/11/10/23452196/elon-musk-twitter-employee-meeting-q-and-a/) and [technical](https://www.technologyreview.com/2022/11/08/1062886/heres-how-a-twitter-engineer-says-it-will-break-in-the-coming-weeks/) problems on top, Mastodon has recived a huge influx of Twitter users fearing that their home of many years is about to implode. A great deal of this influx includes writers, journalist, and other artists. Some companies and organisations have set up their own Mastadon servers, most notably the European Union.

Many others are interested, but are put off by the apparently obtuse way to get on it. This post is for them. I'll detail my experience on the platform, and what I've learned from it. <!--more-->

The first thing I will say is that once you set up an account on Mastadon, it looks *almost* exactly like using Twitter. There are a couple of differences, most of which are deliberate design choices to avoid some of the problems that Twitter faced, but once you set it up, you can use it from the web or an app exactly as you would on Twitter. It's *how* you set up the account that's different. In addition, there are *cultural* differences, which I'll talk about later.

The intial steps in setting up a Mastodon account require a web browser. I'll also be talking about the options for Android and iOS apps later.

## Choosing a server

The first thing you have to do is choose a Mastadon server (often called an "instance") on which to register an account.

This is the bit that I notice flummoxes people the most, and it's especially frustrating as it's flummoxing them right on the first step! If you've read any articles about Mastadon recently, then they will generally do an infodump about Mastodon existing in a "fediverse", a distributed network across different servers. Whilst this is an important technical aspect of the system, such technical details tend to make non-technical people's eye glaze over.

So I would instead liken Mastodon to email. You can create an email account on Gmail or Hotmail, but using that account, you can send emails anywhere outside Gmail or Hotmail as long as you know the email address to send them to. So whether you choose Gmail or Hotmail really depends on which user experience you prefer.

Mastodon is a bit like that. You can create an account on one server, but you can follow people on another as long as you know their Mastodon address. (Which is a bit like an email address.) Once you do their posts will appear on your timeline.

So, having said that, how does one choose a server? I find the most helpful resource at the moment is the [servers list on the official Mastadon site](https://joinmastodon.org/servers). You may notice you can search for servers by special interest subject, or by region. (The UK appear to be ahead on this front at the time of writing.) From here you can select a server, and be taken to it's homepage, where you can sign up.

It may be tempting to sign up to one of the big servers with loads of users, but that might be a mistake. A lot of the big servers are now straining under the huge influx of new users, (Indeed mastodon.social halted new registrations.) and as a result, can be quite slow at times. However, as I mentioned above, you don't *need* to be on a big server to see posts from their users, so it might be a better idea to find a smaller server that runs faster. For example, I picked a server was local to me, and fast.

One thing you might want to do before you sign up is check the Code of Conduct for the site. (This should be in the "About this server" page.) Each site has it's own Code of Conduct: most are anti-hate speech and harrassment, but some sites might vary on this, so check it out just to be sure.

Note that when you sign up, you'll need to put in your email address. You'll also need to decide a username. Note that you can't change it afterwards, so you'll need to choose carefully.

After signing up, there may be some time to wait as some sites have a moderator approve your registration. (These will be the sites on the server list that say "Apply for an account".) Other sites do it automatically. Either way, a verification email is then sent to your email address to allow you to log in.

## Logging in for the first time

After you've logged in, you'll see a very Twitter-like webpage interface, with an area in the top left of the screen for you to compose your posts (Which are called "Toots", although I notice some sites just call them "posts". I know which I prefer.) The first thing you'll want to do is select the "Edit Profile" link, so you can set up your display name, bio, header pic and avatar pic. If you have any links, you can add them in the "Profile Metadata" section. Don't forget to click the "Save changes" button at the bottom.

The next thing to note is when you go to your profile page to see the changes, (Click on the link above "Edit profile".) underneath your display name is your Mastadon address, which will be of the form *"@username@server.name"*. This is address you should be quoting when you are telling people you have joined Mastodon. In fact, you might want to take a quick break, and announce it on Twitter, and pin the tweet to your Twitter profile page as I have done.

## Finding people to follow

This is another initially onerous step. You have a blank timeline staring back at you, and you realise you have to have follow people to see their posts. How do you find them?

Mostodon deliberately makes it harder to find people, in order to prevent the misuse of people searching on Twitter. That means you often find people on Mastodon on a word-of-mouth basis. For example, I found someone I knew, from years back on Flickr and other social media, completely by chance because he was following someone I knew! Here are some strategies I've used to find followers:

1. One way to start is to look at the profile directory on your site. (This should be in the links section in the lower left of the web page.) You can list people from your site, or from across the fediverse. From there, you can directly follow them, or view their posts.
2. If you go into "Local" (From the right hand menu.) you can view posts from users of your own site, and follow people from there.
3. You could also go into "Federated", a timeline of **all** the posts that your site handles in realtime, but that's a bit of a firehose of information, to say the least.
4. Another option (And the nearest thing Mastodon has to an algorithm) is the "Explore" page, which lists currently popular post and hashtags.
5. Indeed, hashtags are a great way to find people to follow.

The point is: you're building up a small amount of people to follow, and from there, you can see who *they* follow, and take things from there. Also, you will have a timeline of their posts, which can contain useful (and fun!) information, especially "boosts" (The equivalent of retweets on Twitter) of cool stuff. One thing I have noticed recently is that if someone famous joins Mastodon, someone in my timeline is talking about it, using that person's Mastodon address, giving me the option of someone new to follow.

### Following someone if you know their Mastodon address

If someone gives you their Mastodon address, or they advertise it on other social media, it's easy- if a little not too obvious- to start following them.

1. Go to the "Search" box on the top left of the screen, and put in the Mastadon address, and click the search icon.
2. The person should come up in the search results. Select this to see their profile
3. Select "Follow".

### Following their followers

You might wonder why this merits it's own section. You just go to the followers list, right?

Well, yes and no. This is one of the more annoying consequences of decentralised structure of Mastodon. You can go to the followers list from your instance, but you only see the followers that *your instance knows about*. (eg people other follow on your instance or whose posts they boost.) For you to see the full list of followers, you must go to the followers page on *their* instance. At the bottom of the followers page on your instance, you will see the following text:

> Followers from other servers are not displayed.
> Browse more on the original profile

... and a link to their profile. So you can browse to their profile, go to their followers page, find someone to follow, and click the follow button, right?

Again, yes and no. In what I consider to be the clunkiest bits of the Mastodon UI experience, when you click the follow button, you will get a popup with a link to copy. (Under the "On a different server" heading.) Once you copy that link, you can paste that link into your search box as above, and follow from there.

It's universally acknowledged that this a super-clunky process, and indeed there are extensions for web browsers like [Google Chrome](https://chrome.google.com/webstore/detail/mastodon-profile-redirect/limifnkopacddgpihodacjeckfkpbfoe) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/mastodon-profile-redirect/) that help smooth over this process.

### Finding followers using Debirdify

Another option is to use a tool like [Debirdify](https://debirdify.pruvisto.org/), where you log in with both your Twitter and Matodon accounts, and it will search for people who you follow on Twitter who announced their Mastdon address, and allows you to download their Mastodon addresses in a handy little CSV file.

Why is a CSV file handy? This next section will tell you...

### Importing a list of followers into your Mastodon account

In Mastodon you can import a list of people to follow from a CSV file, just the ones generated by tools like Debirdify. To do this:

1. Go to "Edit profile".
2. Select the link "Import and Export" from the left hand side.
3. Select the sub-link "Import".
4. You're now in the Import page. Make sure "Following list" dropdown, and "Merge" radio button is selected.
5. You can now select "Choose file" to select your CSV file, and then the "Upload" button to import followers.

## Mastodon Etiquette

One thing you may notice straight away about exploring Mastodon is (At least for now) how *quiet* it is compared to Twitter. The community that built Mastodon, both the developers and the users, regard it as an antidote to the poison and ego in other social media, especially Twitter. This means there are important differences how things work on Twitter.

1. As in the early years of Twitter, your timeline consists of a reverse chronological list of posts from people you follow. There is no algorithm to push other peoples posts to your timeline. The only way you may see other peoples posts is if someone you follow boosts it. That makes boosts more a more powerful way to spread the word in Mastodon than likes. A post can have a lot of likes, but it's only when enough people with enough followers boost it, that it becomes viral in the Mastodon Ecosystem.
2. Another reason it's important to be aware of your instance's moderation policy: individual instances can, and do, block other instances. Usually, it's a case of the mainstream instances blocking shitposter and Nazi instances, including Gab, and Donald Trump's Truth Social. However, users can also block entire instances themselves.
3. It's generally expected that if your post contains an image, you provide an ALT-text, espcially if the image is a paragraph of text!
4. I've seen a lot of use of the Content Warning feature. When you create a post, you can add a content warning. (Click on the "CW" button below the post field.) When you post the post, the main content will be hidden, and the content warning will be shown, along with a button "Show more", which will reveal the main content. I've seen it used for contentious or distressing thems, but I've also seen it used creatively on long posts (Some instances can handle posts of more than 500 characters.) and long threads.
5. You can't do a text search for tweets, but you *can* search for hashtags. This means that using hashtags are more important in Mastodon than they are in Twitter.
6. The vast majority of Mastodon instances are non-profit and are run by people in their spare time, and at their own cost. A lot of them have fund-raisers for costs, or have a payment system to allow people to donate money to costs. If you're getting good useage of out of Mastodon, it is worth considering donating money towards your instance's upkeep. (I leave the irony of paying for Mastodon, whilst running a mile away from doing the same for Twitter, for you to ponder.)

## Crossposting between Twitter and Mastodon

Using Mastodon while still using Twitter can feel a bit like the old days of juggling between MySpace, Bebo and Facebook! Fortunately, (At least, whilst the Twitter API is still working!) there is a [Twitter-Mastodon crossposter service](https://crossposter.jaxbeach.social/) to help post on both platforms. You log in with both your Twitter and Mastodon accounts, and from there you can go to "Options" to configure how you can post between the two platforms.

If you go to "advanced options", you'll find can have quite a lot of control over how the two platforms can interact. I generally configure things so that any tweet or thread I make on one platform appears on the other platforms, any retweet from Twitter goes to Mastodon but not other way around, and that any conservation on one platform stays on that platform.

I would add a note of caution that the Twitter API for free users is generally low bandwidth with a maximum amount of requests per hour, so don't expect to post on one platform, and for it to immediately appear on the other.

## Mastodon apps for mobile devices

For a while, the only way to ineract with Mastodon on a mobile device was through a web browser, (Which was, and still is, a viable option.) and Mastodon's official app didn't arrive until recently, which means that the app ecosystem was largely populated by third party apps which, while they delivered the core functionality, often differed in how they handled some features.

I would probably advise to go for the official Mastodon app for [iOS](https://apps.apple.com/us/app/mastodon-for-iphone-and-ipad/id1571998974) and [Android](https://play.google.com/store/apps/details?id=org.joinmastodon.android&gl=US&pli=1) first, but then try out the other apps after that. Here's a good article on [the iOS apps](https://transponderings.blog/2022/05/21/eight-mastodon-apps-for-iphone/), and one for [Android apps](https://9to5google.com/2022/11/03/best-mastodon-apps-download-android/).

## Beyond Mastodon

Although Mastodon exists in a "fediverse", the fediverse is not just Mastodon. There are a number of other de-centralised social media platforms that are part of the fediverse. For example:

* [Pixelfed](https://pixelfed.org/), an Instagram-like photo sharing platform.
* [Peertube](https://joinpeertube.org/), an YouTube-ish video sharing platform.
* [Funkwhale](https://funkwhale.audio/), a decentralised equivalent to Bandcamp.
* [Matrix](https://matrix.org/), a chat platform, similar to Slack.
* [Frendica](https://friendi.ca/), a Facebook-ish social media platform.
* [WriteFreely](https://writefreely.org/), a blogging platform.
* [Pleroma](https://pleroma.social/), a Mastodon-like social media platform. (!)
* And many more...

What's interesting is that, as they share the same communication protocal, ([ActivityPub](https://www.w3.org/TR/activitypub/)), there is a degree of compatibility between all these platforms. A user in Mastodon, for example, can follow someone on PixelFed, and their PixelFed photos will appear on the user's Mastodon timeline. The user on Mastodon can comment on the photos, and the comments will appear on Pixelfed. This compatibility can be so seamless, you might follow someone on Mastodon for their photos, and only later find out you're following a PixelFed user.

As this Ars Technica article notes, [this interoperability is not 100% perfect](https://arstechnica.com/gadgets/2023/01/mastodon-highlights-pros-and-cons-of-moving-beyond-big-tech-gatekeepers/), but it works well enough to imagine the possiblities of a future where the lines between social media platforms are blurred to the point where you can use one platform to access multiple platforms.

As with Mastodon, the initial step is finding a server, and then finding people to follow. Both [FediDB](https://fedidb.org/) and [Fediverse Party](https://fediverse.party/) are good places to search for servers across the different platforms. Fediverse Party also tells you a bit about each platform, and what platforms are compatible with each other.

One thing to note is that many of these platforms are not quite as mature as Mastodon, and given the spotlight is on Mastodon, that also means there are less users. I suspect that as Mastodon becomes more popular, not only will more people join the other platforms, but the interoperability of these platforms with Mastodon will mean that the growth of Mastodon also leads to the growth of these platforms **as they interact with Mastodon**. If I follow someone on Mastodon for their photos, it doesn't matter to me if I don't know that I've actually followed a user on PixelFed- I liked their photos and therefore followed them. Meanwhile, the user on PixelFed has gained a follower, and the platform has grown a little.

---

Well, this is one of the longer articles I have written for this blog! Making a base on another social media platform can be a bit like moving to another town. It can be a real bother making the actual move, but once you settle down, you start to get used to the place and know where to look for things and who to talk to. That's what I felt, starting out again in Mastodon: it's never going to be the same as Twitter or have exactly the same people that I followed there, but the good things that drew me into Twitter long ago are still there, and it feels it going fine there.
