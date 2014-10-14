---
layout: note
title: HealthKit
---

## Accessing HealthKit

{% highlight swift %}
func authorizationStatusForType(_ type: HKObjectType!) -> HKAuthorizationStatus
{% endhighlight %}

Returns the app’s authorization status for **sharing** the specified data type.

To help prevent possible leaks of sensitive health information, your app **cannot determine** whether or not a user has granted permission to read data. If you are not given permission, it simply appears as if there is no data of the requested type in the HealthKit store.

### `NS_EXTENSION_UNAVAILABLE`

In iOS 8.0, the HealthKit framework is unavailable to app extensions.
