# LaravelFCM\Message\OptionsBuilder | Laravel / Lumen package for Firebase Cloud Messaging    

## [Laravel / Lumen package for Firebase Cloud Messaging](../../index.md)

- [Classes](../../classes.md)
- [Namespaces](../../namespaces.md)
- [Interfaces](../../interfaces.md)
- [Traits](../../traits.md)
- [Index](../../doc-index.md)
- [Search](../../search.md)

>class

>    [LaravelFCM](../../LaravelFCM.md)` / `[Message](../../LaravelFCM/Message.md)` / `(OptionsBuilder)
## OptionsBuilder

class **OptionsBuilder** [View source](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php)



Builder for creation of options used by FCM.


### Properties

|   |   |   |   |
|---|---|---|---|
|<a name="property_collapseKey"></a>protected string|$collapseKey|||
|<a name="property_priority"></a>protected string|$priority|||
|<a name="property_contentAvailable"></a>protected bool|$contentAvailable|||
|<a name="property_mutableContent"></a>protected bool|$mutableContent|||
|<a name="property_delayWhileIdle"></a>protected bool|$delayWhileIdle|||
|<a name="property_timeToLive"></a>protected int|$timeToLive|||
|<a name="property_restrictedPackageName"></a>protected string|$restrictedPackageName|||
|<a name="property_dryRun"></a>protected bool|$dryRun|||
|<a name="property_directBootOk"></a>protected bool|$directBootOk|||
### Methods

|   |   |   |   |
|---|---|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setCollapseKey"></a>setCollapseKey(string $collapseKey)|This parameter identifies a group of messages. A maximum of 4 different collapse keys is allowed at any given time.||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setDirectBootOk"></a>setDirectBootOk(bool $directBootOk)|If set to true, messages will be allowed to be delivered to the app while the device is in direct boot mode.||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setPriority"></a>setPriority(string $priority)|Sets the priority of the message. Valid values are &quot;normal&quot; and &quot;high.&quot;. By default, messages are sent with normal priority.||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setContentAvailable"></a>setContentAvailable(bool $contentAvailable)|support only Android and Ios.||
|OptionsBuilder|<a name="#method_setMutableContent"></a>setMutableContent(bool $isMutableContent)|support iOS 10+||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setDelayWhileIdle"></a>setDelayWhileIdle(bool $delayWhileIdle)|When this parameter is set to true, it indicates that the message should not be sent until the device becomes active.||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setTimeToLive"></a>setTimeToLive(int $timeToLive)|This parameter specifies how long the message should be kept in FCM storage if the device is offline.||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setRestrictedPackageName"></a>setRestrictedPackageName(string $restrictedPackageName)|This parameter specifies the package name of the application where the registration tokens must match in order to receive the message.||
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|<a name="#method_setDryRun"></a>setDryRun(bool $isDryRun)**deprecated**|This parameter, when set to true, allows developers to test a request without actually sending a message.||
|null|string|<a name="#method_getCollapseKey"></a>getCollapseKey()|Get the collapseKey.||
|null|string|<a name="#method_getPriority"></a>getPriority()|Get the priority.||
|bool|<a name="#method_isContentAvailable"></a>isContentAvailable()|is content available.||
|bool|<a name="#method_isMutableContent"></a>isMutableContent()|is mutable content||
|bool|<a name="#method_isDelayWhileIdle"></a>isDelayWhileIdle()|is delay white idle.||
|null|int|<a name="#method_getTimeToLive"></a>getTimeToLive()|get time to live.||
|null|string|<a name="#method_getRestrictedPackageName"></a>getRestrictedPackageName()|get restricted package name.||
|bool|<a name="#method_isDryRun"></a>isDryRun()|is dry run.||
|bool|<a name="#method_isDirectBootOk"></a>isDirectBootOk()|is direct boot ok||
|Options|<a name="#method_build"></a>build()|build an instance of Options.||


### Details
<a name id="method_setCollapseKey"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setCollapseKey**(string $collapseKey)

[at line 85](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L85)

This parameter identifies a group of messages
A maximum of 4 different collapse keys is allowed at any given time.        

#### Parameters

|   |   |   |
|---|---|---|
|string|$collapseKey|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|

<a name id="method_setDirectBootOk"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setDirectBootOk**(bool $directBootOk)

[at line 102](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L102)

If set to true, messages will be allowed to be delivered to the app while the device is in direct boot mode.        See Support Direct Boot mode (https://developer.android.com/training/articles/direct-boot).

#### Parameters

|   |   |   |
|---|---|---|
|bool|$directBootOk|(only true is valid, do not use for false it is pointless)

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|


#### See also
|   |   |
|---|---|
|[https://developer.android.com/training/articles/direct-boot](https://developer.android.com/training/articles/direct-boot)|

<a name id="method_setPriority"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setPriority**(string $priority)

[at line 120](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L120)

Sets the priority of the message. Valid values are "normal" and "high."
By default, messages are sent with normal priority.        

#### Parameters

|   |   |   |
|---|---|---|
|string|$priority|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|


#### Exceptions

|   |   |
|---|---|
|InvalidOptionsException||
|[ReflectionException](https://www.php.net/ReflectionException)||

<a name id="method_setContentAvailable"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setContentAvailable**(bool $contentAvailable)

[at line 142](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L142)

support only Android and Ios.        An inactive client app is awoken.
On iOS, use this field to represent content-available in the APNS payload.
On Android, data messages wake the app by default.
On Chrome, currently not supported.

#### Parameters

|   |   |   |
|---|---|---|
|bool|$contentAvailable|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|

<a name id="method_setMutableContent"></a>

### 
 OptionsBuilder **setMutableContent**(bool $isMutableContent)

[at line 158](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L158)

support iOS 10+        When a notification is sent and this is set to true,
the content of the notification can be modified before it is displayed.

#### Parameters

|   |   |   |
|---|---|---|
|bool|$isMutableContent|

#### Return Value

|   |   |
|---|---|
|OptionsBuilder|

<a name id="method_setDelayWhileIdle"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setDelayWhileIdle**(bool $delayWhileIdle)

[at line 172](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L172)

When this parameter is set to true, it indicates that the message should not be sent until the device becomes active.        

#### Parameters

|   |   |   |
|---|---|---|
|bool|$delayWhileIdle|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|

<a name id="method_setTimeToLive"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setTimeToLive**(int $timeToLive)

[at line 188](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L188)

This parameter specifies how long the message should be kept in FCM storage if the device is offline.        

#### Parameters

|   |   |   |
|---|---|---|
|int|$timeToLive|(in second) min:0 max:2419200

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|


#### Exceptions

|   |   |
|---|---|
|InvalidOptionsException||

<a name id="method_setRestrictedPackageName"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setRestrictedPackageName**(string $restrictedPackageName)

[at line 206](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L206)

This parameter specifies the package name of the application where the registration tokens must match in order to receive the message.        (Android only)

#### Parameters

|   |   |   |
|---|---|---|
|string|$restrictedPackageName|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|

<a name id="method_setDryRun"></a>

### 
 [<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md) **setDryRun**(bool $isDryRun)**deprecated**

[at line 222](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L222)|   |   |
|---|---|
**deprecated**
||v1 (https://stackoverflow.com/a/53885050/5155484)|


This parameter, when set to true, allows developers to test a request without actually sending a message.        It should only be used for the development.

#### Parameters

|   |   |   |
|---|---|---|
|bool|$isDryRun|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Message\OptionsBuilder">OptionsBuilder</abbr>](../../LaravelFCM/Message/OptionsBuilder.md)|

<a name id="method_getCollapseKey"></a>

### 
 null|string **getCollapseKey**()

[at line 234](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L234)

Get the collapseKey.        

#### Return Value

|   |   |
|---|---|
|null|string|

<a name id="method_getPriority"></a>

### 
 null|string **getPriority**()

[at line 244](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L244)

Get the priority.        

#### Return Value

|   |   |
|---|---|
|null|string|

<a name id="method_isContentAvailable"></a>

### 
 bool **isContentAvailable**()

[at line 254](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L254)

is content available.        

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_isMutableContent"></a>

### 
 bool **isMutableContent**()

[at line 264](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L264)

is mutable content        

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_isDelayWhileIdle"></a>

### 
 bool **isDelayWhileIdle**()

[at line 274](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L274)

is delay white idle.        

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_getTimeToLive"></a>

### 
 null|int **getTimeToLive**()

[at line 284](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L284)

get time to live.        

#### Return Value

|   |   |
|---|---|
|null|int|

<a name id="method_getRestrictedPackageName"></a>

### 
 null|string **getRestrictedPackageName**()

[at line 294](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L294)

get restricted package name.        

#### Return Value

|   |   |
|---|---|
|null|string|

<a name id="method_isDryRun"></a>

### 
 bool **isDryRun**()

[at line 304](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L304)

is dry run.        

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_isDirectBootOk"></a>

### 
 bool **isDirectBootOk**()

[at line 314](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L314)

is direct boot ok        

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_build"></a>

### 
 Options **build**()

[at line 324](https://github.com/code-lts/Laravel-FCM/blob/main/src/Message/OptionsBuilder.php#L324)

build an instance of Options.        

#### Return Value

|   |   |
|---|---|
|Options|

_Generated by [Doctum, a API Documentation generator and fork of Sami](https://github.com/code-lts/doctum)._