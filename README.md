<p align="center">
	<img src="https://raw.githubusercontent.com/Marius-brt/42-Intra-Notifier/main/logo.png"
		alt="Logo"
		style="height: 150px; width: 150px" />
</p>

# 42 Intra Notifier

42 Intra Notifier is a small scrapping software that allows you to be notified when you have a new assessment and also to have a reminder 3 minutes before it.

## How to install ?

Go to [release](https://github.com/Marius-brt/42-Intra-Notifier/releases) and choose the latest version corresponding to the OS of your machine (I guess MacOS ?).

> **Google Chrome need to be installed** : If not, install it from the software on your Mac called "*Managed Software Center*".

## How it's working ?

In order to finish the project quickly, I decided to use [Electron](https://github.com/electron/electron) for its simplicity. For the scrapping I use [Puppeteer](https://github.com/puppeteer/puppeteer). It connects to your 42 account and refreshes every 10 seconds the intra homepage. I then use [Cheerio](https://github.com/cheeriojs/cheerio) to get the ratings in the html of the page. The username and password are stored locally on the computer using [Electron Store](https://github.com/sindresorhus/electron-store).

## About 

If you like the project, you can star this repository. If you have an idea to add to the prjoect, feel free to send it in [Issues](https://github.com/Marius-brt/42-Intra-Notifier/issues)