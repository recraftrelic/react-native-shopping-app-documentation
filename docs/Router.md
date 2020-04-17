---
id: Router
title: Router
---

By using router you can easily achieve routing from one page to another page.

## Accessing Routes
Open the Router folder present in the root directory to access the router file.

```
cd router
touch index.tsx
```

```
<ConfigContext.Provider value={configReducer}>
    <ThemedView style={style.container}>
        <NativeRouter>
          <BackHandlerHOC>
            <Switch>
              <Route exact path="/" component={BaseHome} />
              <Route exact path="/base/" component={BaseNext} />
              <Route exact path="/login/" component={Login} />
              <Route exact path="/createAccount/" component={CreateAccount} />
              <Route exact path="/home/" component={Home} />
              <Route exact path="/shopping/" component={Shopping} />
              <Route path="/productDetails/" component={ProductDetails} />
              <Route path="/bag/" component={Bag} />
              <Route path="/payment/" component={Payment} />
              <Route path="/checkout/" component={Checkout} />
              <Route path="/profile/" component={Profile} />
            </Switch>
          </BackHandlerHOC>
        </NativeRouter>
    </ThemedView>
</ConfigContext.Provider>
```

As you can see there are various route defined in the above mentioned file. You can add more route to use in the shopping app.