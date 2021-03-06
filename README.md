# Google Cloud Platform TTS use API-KEY on Android.
## How to use it?

### Step 1: Download file 
```
git clone https://github.com/changemyminds/Google-Cloud-TTS-Android.git
```
### Step 2: Set up API Key
Go to [here](https://github.com/changemyminds/Google-Cloud-TTS-Android/blob/master/app/build.gradle) and change "YOUR_API_KEY" to your Google Cloud API Key. 
```
debug{
    buildConfigField "String", "API_KEY", "\"YOUR_API_KEY\""
}
```

__Note__ <br>
If you don't know the Google API Key, please see [Google document](https://cloud.google.com/docs/authentication/api-keys). <br>

Here prompt the Google API KEY setting. <br>
(1) Got to [google console cloud dashboard](https://console.cloud.google.com/home/dashboard)<br>
(2) Click upper left corner menu and select 'APIs & Services' choose the Credentials.<br>
![image](https://github.com/changemyminds/GCP_TTS_ByAPIKEY/blob/master/images/00.png)<br>
(3) Add CREATE CREDENTIALS and select API Key that will create the no restrict key.<br>
![image](https://github.com/changemyminds/GCP_TTS_ByAPIKEY/blob/master/images/01.png)<br>
(4) Don't forget your API-Key Application restrictions and API restrictions must select _None_ and _Don't restrict key_.<br>
![image](https://github.com/changemyminds/GCP_TTS_ByAPIKEY/blob/master/images/02.png)<br>
 
### Step 3: Run app<br>
See the following achievement.<br>
![image](https://github.com/changemyminds/GCP_TTS_ByAPIKEY/blob/master/images/1.png)<br>
![image](https://github.com/changemyminds/GCP_TTS_ByAPIKEY/blob/master/images/2.png)<br>

## Test language and voice
If you want to test voice or find support language, you can go [here](https://cloud.google.com/text-to-speech/) to test online.

## Reference
[Google Cloud Java Issue](https://github.com/googleapis/google-cloud-java/issues/3400)<br>
[Google Cloud Text-to-speech](https://cloud.google.com/text-to-speech/docs/)<br>
[OkHttp](http://square.github.io/okhttp/)<br>
[Gson](https://github.com/google/gson)

