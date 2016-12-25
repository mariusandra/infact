# infact

This package lets you choose between importing React or Inferno, based on your `BABEL_ENV`

Usage:

```js
// process.env.BABEL_ENV == 'react' || process.env.BABEL_ENV == 'inferno'

import { React, ReactDOM, Inferno, PropTypes, Component } from 'infact'

class MyComponent extends Component {
  render () {
    if (process.env.BABEL_ENV == 'react') {
      // react specific code
    }
    if (process.env.BABEL_ENV == 'inferno') {
      // inferno specific code
    }

    return (
      <div>
        Common code for both
      </div>
    )
  }
}
```
