# 🧠 UIAdView Component

The `UIAdView` component displays ads inside your UI canvas. It is highly configurable through the Inspector.

---

## ✅ How to Add UIAdView from Hierarchy Menu

1. In Unity Editor, go to:

```
GameObject > UI > Magic WebAds > UI Ad View
```

2. This creates a GameObject named **UI Ad View** with the necessary components and attaches it to a Canvas automatically (creates one if none exists).

3. Select the new GameObject to see the properties in the Inspector.

---

## 📸 Screenshot of UIAdView Inspector:

![UIAdView Inspector](../Images/uiadview-inspector.png)

---

## 🗂 Inspector Fields

| Field           | Type               | Description                                                                                   |
|-----------------|--------------------|-----------------------------------------------------------------------------------------------|
| `color`         | `Color`            | Used only in Editor to help design and align ad view dimensions (not visible during runtime).|
| `launchOnEnable` | `bool`             | If true, ad loading will start when the object is enabled.                                   |
| `loadOnEnable`   | `bool`             | If true, the ad request loads automatically when enabled.                                    |
| `showOnLoad`    | `bool`             | Automatically show the ad when loading completes.                                            |
| `hideWhenDisabled` | `bool`          | Hide the ad view when the GameObject is disabled.                                            |
| `filters`       | `List<string>`     | Filters the ads by name to show only matching ads.                                           |
| `adButtons`     | `List<AdButton>`   | Buttons that can trigger ad actions (e.g., click, skip).                                     |
| `listener`      | `UIAdListener`     | Contains all WebView callback events.                                                        |

---

## 📝 Notes

- Add your ad filter names in the `filters` list to restrict which ads are shown.
- Use `adButtons` to add interactive buttons linked to ad actions.
- **Important:** Adjust the `RectTransform` size (`Width` and `Height`) of the UI Ad View GameObject to match the pixel dimensions of your ads for proper display and layout.

---

## 🧩 Next Up:

📄 [Next: AdButtonImage Component](adbuttonimage.md)