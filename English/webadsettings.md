# ⚙️ WebAdSettings Configuration

In the **Magic WebAds** package, the `WebAdSettings` is a `ScriptableObject` that controls how the WebView ad should behave and look. These settings can be shared across different ad requests and services.

---

## ✅ How to Create WebAdSettings

1. Right-click inside the `Project` window
2. Navigate to:

> `Create > Magic WebAds > WebAdSettings`

3. A new ScriptableObject will be created
4. Rename it (e.g. `CryptoWebSettings`)
5. Select it and configure it in the **Inspector**

---

## 🖼 Full Inspector View

![WebAdSettings Inspector](../Images/webadsettings-inspector.png)

---

## 🗃 WebAdSettings Parameters Table

| Field Name              | Type     | Description                                                             |
|-------------------------|----------|-------------------------------------------------------------------------|
| `openLinksInSystemBrowser` | `bool`   | Opens links in system browser instead of WebView                        |
| `isTransparent`         | `bool`   | Makes the WebView background transparent (if supported)                |
| `enableJavaScript`      | `bool`   | Enables JavaScript execution in the WebView                            |
| `enableZoom`            | `bool`   | Allows zooming in/out inside the WebView                               |
| `enableScroll`          | `bool`   | Enables scrolling (vertical & horizontal)                              |
| `allowMixedContent`     | `bool`   | Allows both HTTP and HTTPS content                                     |
| `useCustomUserAgent`    | `bool`   | Enables use of a custom User-Agent string                              |
| `customUserAgent`       | `string` | The custom User-Agent string to apply                                  |
| `enableCookies`         | `bool`   | Enables cookies support in the WebView                                 |
| `cacheEnabled`          | `bool`   | Enables internal caching for faster loading                            |
| `clearCacheOnStart`     | `bool`   | Clears cache before each ad load                                       |
| `fitContentToView`      | `bool`   | Scales content to fit exactly inside WebView                           |
| `disableUserZoom`       | `bool`   | Disables user zoom gestures (e.g., pinch)                              |
| `maintainAspectRatio`   | `bool`   | Maintains aspect ratio when scaling content                            |

---

## 🧩 Next Up:
📄 [Next: Canvas Configuration Guide](canvas-setup.md)