---
layout: post
title: "Create a Floating Pinned Fluid App"
date: 2014-03-14 00:42:57
categories: tutorials
---

This is a tutorial on how to create an app using [Fluid][fluidapp] that is pinned to your status bar and floats above all other windows. My specific goal in doing this was to create an app with a bunch of cheat sheets in it that I could quickly open with a keyboard shortcut, glance at whatever I couldn't remember, and then quickly dismiss the app. I want to do this all without any disruption to whatever task I am in the middle of.

## What is Fluid?

![Fluid App](/img/fluid_logo_icon.png)

If you already know what Fluid is, jump to the next section. For those that haven't heard of Fluid before, stay right here. Fluid is a nifty OS X app that lets you turn any website into a dedicated app on your Mac. For example, say you want to turn Gmail into an app that lives in your `Applications` folder, `.app` extension and all, so that you can launch it independently of everything else, use the task switcher to jump to it, and see it in your dock. This makes sense. There are many web applications that are much like regular desktop apps, Gmail, Google Calendar, and GitHub are good examples. As a native desktop app you can close it with `command+Q`, you can start the app with Spotlight by typing `command+space` and then typing the name of your app.

I've found that some of the best candidates for Fluid are web apps that provide their own set of keyboard shortcuts. This allows you to seamlessly `command+tab` to the dedicated Fluid app and just use your keyboard to navigate within the app itself. 

![Task switcher](/img/suugithub.jpg)

For example, I created an app for GitHub using Fluid. I like using my keyboard as much as possible and avoiding the mouse whenever I can. This allows me to `command+tab` to my GitHub app and then type `G C` to go to the code view in GitHub. I can then type `G P` to go to pull requests, use `J` and `K` to navigate between open pull request. To view a pull request, I simply hit `return` on the highlighted pull request. The dedicated GitHub app removes a little bit of friction vs going to my browser, finding which tab or tabs have GitHub open.

## Pinned to your status bar

Another use case for Fluid is to turn a website or web app into a dedicated desktop app and then take it a step further by putting it in the status bar at the top of your Mac's screen. Once it is there, you can do a couple of cool things. You can assign a keyboard shortcut to activate it and you can also make it appear on any desktop you happen to be on and even make it float above all other windows.

This is perfect for something you would want quick access to no matter what desktop you happen to be on. You could do this with your email, your calendar, or a cheat sheet like I have done. I used this approach to make use of [Brett Terpstra's][brettterpstra] project [Cheaters][cheaters], a customizable cheat sheet system.

### Step 1: Create your app

[Download Fluid][fluidapp] if you haven't already. It is free, but in order to pin your app to the status bar, you will need to pay for it. It is only $5.

* Launch Fluid
* Enter the URL of your website or page.
* Choose an icon.
* Save to your `Applications` folder.

When you first launch Fluid, you will get a simple dialog box that allows you to enter the URL of the web page / web app, give it a name, and select an icon. By default it grabs the website's favicon, but you can use whatever you want.

![Create an app](/img/fluid_create_app.png)

### Step 2: Launch your app and pin it to the status bar

* Launch your app.
* Open the application menu (click the app name in the status bar).
* Choose `Pin to Status Bar...`.  
> **note:** you won't see this option unless you've paid $5 to unlock the extra features.
* Confirm that you want it in the status bar.

![Pin to status bar](/img/fluid_pin_to_status_bar.png)

It will end up looking like this, but with whatever icon you chose for your app.

![App in status bar](/img/fluid_pinned_app.png)

Clicking on the icon will activate the app. You will see a window pop open with your website / webapp neatly displayed inside.

### Step 3: Make it float and assign a keyboard shortcut

The final step is to make your app float and assign it a keyboard shortcut. Making your app float is so that it will appear on whichever desktop you happen to be on and it will hover nicely above any other open apps.

* Open your app's preferences `command+,` when your app is active.
* Go to `Appearance`
* Under the `Window Level` option choose `Floating`

Without setting the window level to **Floating** when you activate your app, it will jump you to whatever desktop you happened to be on when you pinned the app to the status bar in the first place. We want to avoid that kind of jarring experience. We don't want to be ripped away from what were doing and then have to find our way back. What we are shooting for is a quick glance and then dismiss it with no disruption to the flow of whatever task you were doing.

![Floating](/img/fluid_floating.png)

Next, assign a keyboard shortcut to quickly activate your app. Assigning a keyboard shortcut gets us closer to the desired behavior of quickly activating and then dismissing the app.

* In Preferences, go to `General Preferences` and set a `Global Shortcut`

![Keyboard shortcut](/img/fluid_keyboard_shortcut.png)

## Finished

You can now activate your app with your keyboard shortcut and it will be ready for you on any desktop that you are on. Hitting `esc` or hitting your keyboard shortcut again will make it disappear and you can go right back to whatever you were doing before. It is frictionless access to your app.

I use this to activate my cheat sheets. It contains reference material for all kinds of stuff. It is exactly the type of thing you would want to quickly access and then dismiss without jumping to another desktop or task switching.

Below is a screenshot of my app activated. I could see this approach being useful for quickly accessing your email or calendar also.

![Active app](/img/fluid_pinned_app_active.jpg)

[brettterpstra]: http://brettterpstra.com/
[fluidapp]: http://fluidapp.com/
[cheaters]: http://brettterpstra.com/2012/03/04/cheaters-customizable-cheat-sheet-system/



