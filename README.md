# Firefox Theme
---
### How can we check the theme in firefox?
**1** Open Firefox

**2** Type in the address bar:
```
about:debugging#/runtime/this-firefox
```

**3** Click “Load Temporary Add-on”

**4** Select your manifest.json

**5** Boom. Theme applies instantly

---

### manifest.json file structure
A Firefox theme is a type of WebExtension, so it uses a manifest.json file.
Here is the structure:
```
manifest.json
│
├── manifest_version  (required)
├── name              (required)
├── version           (required)
├── description       (optional but recommended)
│
└── theme             (required for themes)
    ├── colors        (optional but most common)
    └── images        (optional)

```
#### Minimum required fields for a theme:
```
{
  "manifest_version": 2,
  "name": "Theme Name",
  "version": "1.0",
  "theme": {
    "colors": { ... }
  }
}
```
---
#### Optional fields:

**description** (for the add-ons page)

**icons** (for add-on icon, not needed for themes)

**images** (for background images)

---

### keys description

**frame** : Top frame color

**frame_inactive** : Frame color when unfocused

**toolbar** : Toolbar background

**toolbar_text** : Toolbar text color

**tab_background_text** : Inactive tab text

**tab_background** : Inactive tab background

**tab_text** : Active tab text

**tab_selected** : Active tab background

**tab_selected_text** : Active tab text

**toolbar_field** : Address bar background

**toolbar_field_text** : Address bar text

**toolbar_field_border** : Address bar border

**popup** : Popup background

**popup_text** : Popup text

**sidebar** : Sidebar background

**sidebar_text** :  Sidebar text

**toolbar_field_text** : Top frame image

**theme_frame** : Toolbar image

**theme_toolbar** : New tab background image

**theme_ntp_background** :New tab background image

**theme_ntp_attribution** : New tab credit image

**theme_tab_background** : Tab background image

**theme_sidebar** : Sidebar image

**theme_sidebar_header** : Sidebar header image

**theme_bookmarks_toolbar** : Bookmarks bar image

**theme_icons** : Custom icons

**ntp_background** : new tab background color

**ntp_text** : new tab text

---
