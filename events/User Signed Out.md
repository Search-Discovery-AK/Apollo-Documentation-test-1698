# User Signed Out

## Javascript Code
```js
window.appEventData1698 = window.appEventData1698 || [];
appEventData1698.push({
  "event": "User Signed Out",
    "user": {
        "custKey": "<custKey>",
        "loginStatus": "<loginStatus>",
        "profileAttributesList": "<profileAttributesList>",
        "system": "<system>",
        "userType": "<userType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|custKey|string|Unique identifier of a customer.  Any id's considered PII must be hashed. ||||||||
|loginStatus|string|Describes the login state of the user|logged in, logged out, guest|||||||
|profileAttributesList|string|A twice delimited string of key / value pairs.  Use ~ between key and value.  Use | between pairs|homeStore~234|loyaltyTier~gold|memberSince~2002|||||||
|system|string|Describes the system that the user is logged into.  (rarely used). |admin, shop, member|||||||
|userType|string|Describes the type of the user.  Often used to differentiate customers from employees or associates. |employee, guest, agent, customer|||||||
