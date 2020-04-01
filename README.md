# VanillaJavaScriptConfig

> Deliver experiences best suited to a user&#x27;s OS, device type, browser, and other things

[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)

This is a suite of [Vanilla JavaScript](http://vanilla-js.com/) and utilities for loading based on a user's:
- Operating System
- Browser
- Configuration

## Objective
Make it easier for developer to target different devices based on their configuration. It can be used to check different settings related to config in order to deliver best experiences to user.  

## Loading

```jsx
    <script src="./VanillaJavaScriptConfig.js"></script>
```

## Usage



### Operating System

```jsx

const [os,isWin,isMac,isUnix,isLinux,isWinMob,isAndroid,isiOS] = checkOS();
 
```

|  Value   |      Returns        |  Return type |
|----------|:-------------------:|------:|
|    `os`    | Returns the name of OS | String |
| `isWin` | Returns true if OS is Windows and vice versa        |   boolean |
| `isMac` | Returns true if OS is Mac and vice versa       |    boolean |
| `isUnix` | Returns true if OS is Unix and vice versa       |    boolean |
| `isLinux` | Returns true if OS is Linux and vice versa       |    boolean |
| `isWinMob` | Returns true if OS is Windows Mobile and vice versa       |    boolean |
| `isAndroid` | Returns true if OS is Android and vice versa       |    boolean |
| `isiOS` | Returns true if OS is iOS and vice versa       |    boolean |
&nbsp;

___

### Browser

```jsx

const [browser,isChrome,isFirefox,isIE,isEdge,isSafari,isOpera,isYandex] = checkBrowser();
 
```

|  Value   |      Returns        |  Return type |
|----------|:-------------------:|------:|
|    `browser`    | Returns the name of browser | String |
| `isChrome` | Returns true if browser is Chrome and vice versa        |   boolean |
| `isFirefox` | Returns true if browser is Firefox and vice versa       |    boolean |
| `isIE` | Returns true if browser is IE and vice versa       |    boolean |
| `isEdge` | Returns true if browser is Edge and vice versa       |    boolean |
| `isSafari` | Returns true if browser is Safari and vice versa       |    boolean |
| `isOpera` | Returns true if browser is Opera and vice versa       |    boolean |
| `isYandex` | Returns true if browser is Yandex and vice versa       |    boolean |
&nbsp;

___

### Config

```jsx

const [deviceConfig,isCookieEnabled,isOnLine,knownLangs,prefLang,isJavaEnabled] = checkDeviceConfig();
 
```

|  Value   |      Returns        |  Return type |
|----------|:-------------------:|------:|
|    `deviceConfig`    | Returns the different properties (`isCookieEnabled`,`isOnLine`,`knownLangs`,`prefLang`,`isJavaEnabled`) related to config | Arrays of objects |
| `isCookieEnabled` | Returns true if cookie is enabled and vice versa        |   boolean |
| `isOnLine` | Returns true if user is online and vice versa        |   boolean |
| `knownLangs` | Returns an array representing the languages known to the user, by order of preference |   array |
| `prefLang` | Returns an string representing the preferred language of the user, usually the language of the browser UI. The null value is returned when this is unknown.  |  String |
| `isJavaEnabled` | Returns true if Java is enabled and vice versa        |   boolean |

&nbsp;

___


## License

MIT © [usamnet000](https://github.com/usamnet000)

