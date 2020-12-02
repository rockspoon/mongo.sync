# mongo sync

To clone in real time using mongo stream a cluster into another cluster with the option to change the database name and the collection name.

## How to run it

- Create a file similar to options.js at the root folder and set the right configuration 
- Set an environment variable to point to this file
- run the code

here is a bash script example 
```bash
export SOAJS_MONGO_SYNC_OPTIONS=options.js

node main.js
```

### Environment variables
ENV Variable | Description | Default
--- | ----- | :---:
SOAJS_MONGO_SYNC_OPSTIME | 0 = turned off, 1 = get time from ops col, 2 = use time from options | 0
SOAJS_MONGO_SYNC_DEBUG | 0 = turned off, 1 = turned on | 0
SOAJS_MONGO_SYNC_OPTIONS | check options.js | no default, required


### License
*Copyright SOAJS All Rights Reserved.*

Use of this source code is governed by an Apache license that can be found in the LICENSE file at the root of this repository.
