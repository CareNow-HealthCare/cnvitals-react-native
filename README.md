# Carenow-CarePlixVitals React-Native SDK

Although this Cordova plugin is public, you'll need a license for the [CNVitals SDK](http://www.carenowvitals.com/) in order to use it.
If you have a license you'll need to clone this repository and replace the library/framework files with the ones you received from CarePlix Team.

## Installation

To install the plugin to your React Native project use the CLI Tool:

```
#!bash
$ npm i react-native-cnvitals-react-native
```

#### Full example

```javascript
onDeviceReady: function() {
  // Start measurement, the measurement will stop automatically on the end.
    let data = JSON.stringify({
      api_key: '',
      scan_token: '',
      user_id: '',
    });
    CnvitalsReactNative.getVitals(data).then(setResult);

  //successCallback
  The function to be executed when the reading has successfully completed or failed
  setResult(values){
      //where the values are the various measurements obtained or the error occured 
      [JSON Object String]
  }

  //params
  The various key params to be passed to make the sdk work
  {
      api_key : "sample_key",
      scan_token : "sample_token",
      user_id : "sample_user_id"
  } 
});
````
#### For any Queries

You can also refer to the example application which is inside the package for any dounbts regarding the setup or dependencies

#### For any Queries

Please visit the [Carenow](https://www.carenow.healthcare).
Contact customer support for obtaining the sdk
(mailto:help@carenow.healhcare)
