# Few lines to import C/C++ functions

```go
// #cgo CFLAGS: -g -Wall
// #include <stdlib.h>
// #include "file_name.h"
import "C"
```

-g - enables debug symbols
-Wall - enables all warnings
