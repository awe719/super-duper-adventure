# One Code Apps For Android

{% hint style="warning" %}

#### **Minimum Required SDK Version**

One code apps is supported starting Android SDK v15.0.0
{% endhint %}

### Overview

The **One Code Apps** feature enables teams with **shared code base applications** to integrate multiple app variants under a single Luciq app token. This is ideal for organizations that release the same app to different brands, markets, or regions but want to consolidate stability and performance monitoring.

Instead of creating a separate Luciq application for each variant, you integrate all variants using **one Luciq app token** and identify each variant via the **bundle-id using the App variant API**.

### Integrating One Code Apps

{% stepper %}
{% step %}

#### Get Your Luciq App Token

From your Luciq dashboard, go to your application’s settings and copy the **app token** — this will be used for all variants.
{% endstep %}

{% step %}

#### Set the App Variant Name

Call the method before initializing the SDK:

{% code title="Kotlin" %}

```kotlin
Luciq.Builder(this, "token")
        .setAppVariant("bundle-id/brand-name")
        .build()
```

{% endcode %}
{% endstep %}
{% endstepper %}

{% hint style="success" %}

#### **Best Practice**

Use the **same variant name format** across all apps (e.g., bundle ID or a consistent naming convention) to make filtering easier in the dashboard.

We recommend using the unique part of the the bundle-id, assume your bundle-id is: com.example.123245r454523452.MyApp.US, we recommend setting the app variant as ***MyApp US***.
{% endhint %}
- 👋 Hi, I’m @Honesty47
- 👀 I’m interested in ...Dance
- 🌱 I’m currently learning ...code
- 💞️ I’m looking to collaborate on ...Anything i can learn
- 📫 How to reach me ... awebea49@gmail.com
- 😄 Pronouns: ...She/her
- ⚡ Fun fact: ...I'm a nurse. Comedian

<!---
Honesty47/Honesty47 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
