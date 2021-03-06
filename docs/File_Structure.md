---
id: Folder_Structure
title: Folder Structure
---

After creation, your project should look like this:

```
recraft-react-native-shopping-app/
  README.md
  App.tsx
  index.js
  node_modules/
  package.json
  android/
  ios/
  config/
    AppConfigProvider.ts
    DefaultConfig.ts
    themes.ts
    language.ts
    language/
      en.ts
      fr.ts
    ...
  util/
    index.ts
  hooks/
    useBackHandler.tsx
    useConstants.ts
    useTheme.tsx
  router/
    index.tsx
  store/
    index.ts
    reducers/
      config.ts
  pages/
    Home/
      index.tsx
      HomePageProducts.tsx
    BaseHome/
      index.tsx
    ...
  components/
    Base/
      BagItem.tsx
      ButtonItem.tsx
      BagOption.tsx
    ...
    HOC/
      BackHandlerHOC.tsx
    UI/
      ThemedText.tsx
      ThemedView.tsx
    common/
      BackButton/
      Carousel/
      Main/
    Modal/
      CommonModal.tsx
```

For the project to build, these files must exist with exact filenames:

* App.tsx is the page template;
* index.js is the JavaScript entry point.

You can delete or rename the other files.

You may create subdirectories inside src. For faster rebuilds, only files inside src are processed by webpack. You need to put any JS and CSS files inside src, otherwise webpack won’t see them.

You can, however, create more top-level directories. They will not be included in the production build so you can use them for things like documentation.

If you have Git installed and your project is not part of a larger repository, then a new repository will be initialized resulting in an additional top-level .git directory.
