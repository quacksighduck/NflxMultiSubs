<p align="center"><a href="README.md">English</a>, <a href="README_cn.md">中文</a></p>


<img src="docs/icon.png?raw=true" height="48"> NflxMultiSubs
============================================================
Best ever Chrome/Firefox extension to unleash bilingual subtitles on Netflix!


[![Download on Chrome Web Store](docs/chrome-webstore-badge58.png?raw=true)](https://chrome.google.com/webstore/detail/pjhnilfooknlkdonmjnleaomamfehkli/)



Features
--------
- Enable secondary subtitles in all languages (incl. image-based subtitles like Japanese, Chinese, Russian, …)
- Smart selection on secondary subtitles: automatically switch to Japanese for Japanese anime, English for US TV shows
- Seamless integration with native Netflix player UI -- switch languages in place
- Adjust playback speed (pressing key `[` and `]`)
- Open source!!



See it in Action
----------------
![Bilingual Subtitles with zh-tw/jp](docs/zh-ja.jpg?raw=true)
![Intergrated in original menu](docs/popup-menu.jpg?raw=true)


Build
-----
Requires Node.js. Build directories are `build/chrome` and `build/firefox`.
```
git clone https://github.com/gmertes/NflxMultiSubs.git
cd NflxMultiSubs
npm install
npm run build
```

Known Issues
-------------------------
- Refresh the page if the secondary sub list is empty.
- This extension could conflict with other Netflix-related extensions. If you encounter any problem, try to disable some of them
- This extension could conflict with ad blockers (e.g. [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)); Please add `netflix.com` into their whitelists or disable the ad blockers
- RTL (right-to-left) text-based subtitles are not ready yet
- This extension and the developers are not affiliated with Netflix, Inc; All rights belong to their owners


Problems?
---------
### The secondary subtitles list is empty
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


Licenses
--------
MIT. Refer to [LICENSE.md](LICENSE.md) for details
