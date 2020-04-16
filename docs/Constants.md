---
id: Constants
title: Constants
---

By using constants you can easily manage & access the static values or items throughout the app.

## Accessing Constants
Open the config folder present in the root directory to access the constants file.

```
cd config
touch DefaultConfig.ts
```

```
// @ts-ignore
const Logo = require("../images/recraftshoping-app-logo2.png")

export const defaultConfig: ApplicationConfig = {
    constants: {
      selectedTheme: ThemeKey.light,
      selectedLanguage: LanguageKey.en,
      title: "RecraftShoppify",
      recraftLogo: Logo,
      homePage: {
        productLabel: "NEW",
        labelViewAll: "View All",
        labelFashion: "FASHION",
        labelSave: "SALE",
      },
      advertisement: {
        label1: "SHOP",
        label2: "NOW",
        labelBuy: "BUY",
      },
    },
}
```

As you can see there are various predefined constants in the above mentioned file. You can add more constants to use in the shopping app.
