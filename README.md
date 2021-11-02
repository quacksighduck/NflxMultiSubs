<p align="center"><a href="README.md">English</a>, <a href="README_cn.md">中文</a></p>


<img src="docs/icon.png?raw=true" height="48"> NflxMultiSubs
============================================================
Best ever Chrome/Firefox extension to unleash bilingual subtitles on Netflix! 

This repository is updated for 2021 with a fix for the Netflix redesign and other bug fixes and improvements.

[<img src="https://user-images.githubusercontent.com/13658335/138092194-303708fb-9a4e-4e3f-a1dc-74baff1e45c9.png" height="59"/>](https://chrome.google.com/webstore/detail/jepfhfjlkgobooomdgpcjikalfpcldmm)
[<img src="https://user-images.githubusercontent.com/13658335/138086366-8deee659-16c3-4621-b3f0-eaf4cb6ed9ba.png" height="60"/>](https://addons.mozilla.org/en-GB/firefox/addon/nflxmultisubs-2021)

#### UPDATE: We are now on the Chrome and Firefox stores under the name NflxMultiSubs 2021 🥳🥳🥳 <br /> Click the browser badge to install.

**If you manually installed the extension before, please remove it and reinstall from the store.**

Features
--------
- Enable secondary subtitles in all languages (incl. image-based subtitles like Japanese, Chinese, Russian, …)
- Smart selection on secondary subtitles: automatically switch to Japanese for Japanese anime, English for US TV shows
- Seamless integration with native Netflix player UI -- switch languages in place
- Adjust playback speed (pressing key `[` and `]`)
- Open source!!

Build
-----
Requires Node.js. Build directories are `build/chrome` and `build/firefox`.
```
git clone https://github.com/gmertes/NflxMultiSubs.git
cd NflxMultiSubs
npm install
npm run build
```

How to manually install the extension
-----
See [INSTALL.md](INSTALL.md) for instructions.

See it in Action
----------------
![Bilingual Subtitles with zh-cn/en](docs/2021_zh-en.jpg?raw=true)
![Intergrated in original menu](docs/2021_popup-menu.jpg?raw=true)
![Settings menu](docs/2021_settings.jpg?raw=true)


Known Issues
-------------------------
- Wait for the Netflix home page to finish loading completely before starting a show/movie.
- Refresh the page if the secondary sub list is empty.
- This extension could conflict with other Netflix-related extensions. If you encounter any problem, try to disable some of them
- This extension could conflict with ad blockers (e.g. [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)); Please add `netflix.com` into their whitelists or disable the ad blockers
- RTL (right-to-left) text-based subtitles are not ready yet
- This extension and the developers are not affiliated with Netflix, Inc; All rights belong to their owners


Problems?
---------
### The secondary subtitles list is empty or subs aren't showing up
- Subs will show up after a Refresh (F5).

### Netflix player keeps loading, and error messages occurs afterward
- Try hitting Refresh (F5) few times
- Loading could be interfered by ad blockers -- add `netflix.com` to their whitelist or disable the ad blockers temporarily

### Large gap between main subtitle and secondary subtitle
- Sometimes this happens only when the controls bar is active -- just wait until the controls hide

### Main subtitle moved to center of the visible region
- Sometimes this happens only when the controls bar is active -- just wait until the controls hide

### Only available in Chrome for desktop?
- Yup -- mobile devices, smart TVs, Apple TV, Chromecast, … are not supported
- No plan to support those platforms -- request Netflix to deliver official supports ;-)

### Could I load subtitles from other country?
- This extension respects Netflix rules, hence we only support all official subtitles available in your country
- Uploading custom subtitles won't be supported

### Feature request: __________ ?
- This extension does one thing and does it well -- great experience with bilingual subtitles support
- If you have a request you can open an issue for consideration (please put [Feature Request] in the title)


License
--------
MIT. Original by [Dan Chen](https://github.com/dannvix), forked and maintained by [Gert Mertes](https://github.com/gmertes).
