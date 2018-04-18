# angular-aframe-pipe

A-Frame pipe for Angular

[![Build Status](https://travis-ci.org/urish/angular-aframe-pipe.png?branch=master)](https://travis-ci.org/urish/angular-aframe-pipe)

Installation
------------

`npm install --save angular-aframe-pipe`

Usage
-----

Import `AframePipeModule` into your app's modules:

``` typescript
import { AframePipeModule } from 'angular-aframe-pipe';

@NgModule({
  imports: [
    AframePipeModule
  ]
})
```

This makes all the `aframe` pipe available for use in your app components.

Using the pipe
--------------

Use the pipe whenever you need to pass a custom value as an attribute to a-frame element in your Angular template:

```html
<a-sphere [attr.position]="{x: 0, y: height, z: 0} | aframe">
</a-sphere>
```

This will set the height of the sphere dynamically, based on the `height` property of your component.

License
-------

MIT. Copyright (C) 2018, Uri Shaked.
