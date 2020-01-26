# x-www-form-urlencoded-post-in-react-native

```
var details = {
    'userName': 'admin@gmail.com',
    'password': 'Password!'
};

var formBody = [];
for (var property in details) {
  var encodedKey = encodeURIComponent(property);
  var encodedValue = encodeURIComponent(details[property]);
  formBody.push(encodedKey + "=" + encodedValue);
}
formBody = formBody.join("&");

fetch('http://identity.azurewebsites.net' {
  method: 'POST',
  headers: {
    'Accept': 'application/json',
    'Content-Type': 'application/x-www-form-urlencoded'
  },
  body: formBody
})
```
