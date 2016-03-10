# easysort
Easy sort in Go

## Example

```go

import (
	"fmt"
	"github.com/miolini/easysort"
)

type User struct {
	Name string
	Age  int
}

func main() {
	users := []User{ User{"testa", 45}, User{"testb", 30} }
	easysort.ByField(users, "Age")
	fmt.Println(users)
}
```