# This is how you do it!

run.sh
```docker

#!/bin/bash

set -e

pio-start-all
pio app new something
cd /YourProject
pio build --verbose


```

``` docker

FROM atyz/predictionio

ADD YourProject /YourProject

EXPOSE 8000

ADD run.sh /run.sh

ENTRYPOINT /run.sh

```
