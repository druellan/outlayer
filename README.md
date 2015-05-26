# Outlayer fork

This is a fork of the Outlayer project (https://github.com/metafizzy/outlayer).

### New Features

##### New `lock` property
Specifies elements are *locked* within the layout. These are special layout elements which will **be** laid out by Packery, but could have some restrictions on their behaviour.

```
"itemSelector": ".item",
"lock": ".locked"
```

#### New `reloadContent` method
This method is similar to `reloadItems`, but the function also identifies new items with the `stamp` and `lock` properties, that otherwise are only parsed during the initialization.

```
$container.packery('reloadContent')
// or with vanilla JS
pckry.reloadContent()
```