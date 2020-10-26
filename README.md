React Native Pushwoosh Baidu Push Notifications module
===================================================

| [Guide](https://docs.pushwoosh.com/platform-docs/pushwoosh-sdk/android-push-notifications/baidu-integration) | [Documentation](docs/README.md) | [Sample](https://github.com/Pushwoosh/pushwoosh-react-native-baidu-sample) |
| ----------------------------------------------------------- | ------------------------------- | -------------------------------------------------------------------- |


### Installation

```
npm install pushwoosh-react-native-baidu-plugin --save
react-native link pushwoosh-react-native-baidu-plugin
```

### Usage

```js
import Pushwoosh from 'pushwoosh-react-native-baidu-plugin';

Pushwoosh.init({ 
    "pw_appid" : "YOUR_PUSHWOOSH_PROJECT_ID" , 
    "baidu_api_key" : "YOUR_BAIDU_API_KEY" 
});
Pushwoosh.register();
```

In order to use reverse proxy to connect to pushwoosh servers specify the parameter "reverse_proxy_url" with the url to your reverse proxy when initializing the plugin:

```js
import Pushwoosh from 'pushwoosh-react-native-baidu-plugin';

Pushwoosh.init({ 
    "pw_appid" : "YOUR_PUSHWOOSH_PROJECT_ID" , 
    "baidu_api_key" : "YOUR_BAIDU_API_KEY",
    "reverse_proxy_url" : "URL_TO_YOUR_REVERSE_PROXY"
});
Pushwoosh.register();
```
