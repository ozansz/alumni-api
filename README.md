# alumni-api

RESTful API server for IEEE METU CS Alumni Project, running Express.js on Node.js

## Installation

```bash
git clone https://ieee-odtu/alumni-api
cd ./alumni-api
npm install
npm run dev
```

### for developers

For a better development process, add the lines below right after line #240 in express/lib/response.js

```js
val.debug = val.debug || {};
if (['POST', 'PUT', 'PATCH'].includes(this.req.method)) {
  val.debug.body = this.req.body;
}
```

<hr></hr>

**This repository is part of IEEE METU CS Alumni Project and has been licensed under The MIT License.**
