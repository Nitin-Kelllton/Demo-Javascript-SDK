
# Javascript Sdk

The Javascript SDK for JavaScript doesn't have any standalone files that need to be downloaded or installed, instead you simply need to include a short piece of regular JavaScript in your HTML that will asynchronously load the SDK into your pages. The async load means that it does not block loading other elements of your page.

------------------


<a name="usage"></a>
### Getting Started
1. You will need to contact partners@xyj.com to receive a partnerID

2. Once you receive a partnerID, you can start to integrate the SDK into your app frontend.

Add sdk url to your script tag 

```javascript

  <script src="_sdk_min.js"></script>

```

For initialising javascript sdk in your website in <script> tag

```javascript

<button id="buy-button1">Buy</button>
document.getElementById('buy-button1').onclick = function(e){
  
  var sdk = new ClientSdk()
  sdk.init({
    partnerID: "",
    productId: "",
    callBack: "",
    errorhandler: ""
  })
  sdk.openWindow(); //This will prompt Iframe window where we can proceed for product buying journey process
}
```

| Parameter | Required? | Default | Type | Description
|:---|:---:|:---|:---|:---|
| partnerID | Yes | `""` | `string` | - |
| productId | Yes | `-` | `string` |- |
| callBack | No | `-` | `funtion` | Fucntion will be called to push events update | 
| errorhandler | No | `-` | `funtion` | Fucntion will be called to notify any error | 



<a name="authors"></a>
### Authors

