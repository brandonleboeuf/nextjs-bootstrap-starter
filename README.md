## Next.js Bootstrap
Basic starter for Next.js and Bootstrap

_Install_
```npm i bootstrap```
```npm install @popperjs/core --save```

_Update_
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