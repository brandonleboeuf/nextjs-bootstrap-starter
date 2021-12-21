## Next.js Bootstrap
Basic starter for Next.js and Bootstrap

## Install
```npm i bootstrap```

```npm install @popperjs/core --save```

## Update
```jsx
import "bootstrap/dist/css/bootstrap.css";
import "../styles/globals.css";

import { useEffect } from "react";

function MyApp({ Component, pageProps }) {
  useEffect(() => {
    import("bootstrap/dist/js/bootstrap");
  }, []);

  return <Component {...pageProps} />;
}

export default MyApp;
```