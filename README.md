# OneTab Merge

Util for [OneTab browser extension](https://www.one-tab.com).

Merge different sources preserving time order.

## Install

in cloned folder, do `npm install`

## Usage

* Get the HTML of all your OneTab pages
* Merge them
* Close your browser and delete OneTab files
* Import the merge result into OneTab

**Merge**

```sh
./merge-html html/*
./merge-html onetab-osx-chrome.html onetab-osx-firefox.html onetab-linux-chromium.html
```

**OneTab files**

Chrome OSX
```
~/"Library/Application Support/Google/Chrome/Default/Local Storage/chrome-extension_chphlpgkkbolifaimnlloiipkdnihall_0.localstorage"
~/"Library/Application Support/Google/Chrome/Default/Local Storage/chrome-extension_chphlpgkkbolifaimnlloiipkdnihall_0.localstorage-journal"
```

Chromium Linux
```
~/".config/chromium/Default/Local Storage/chrome-extension_chphlpgkkbolifaimnlloiipkdnihall_0.localstorage"
~/".config/chromium/Default/Local Storage/chrome-extension_chphlpgkkbolifaimnlloiipkdnihall_0.localstorage-journal"
```

Firefox Linux
```
`find ~/.mozilla/firefox -maxdepth 1 -type d -name *.default`/storage/permanent/indexeddb+++extension-at-one-tab-dot-com/
```
