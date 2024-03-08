<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	testpetstorego "github.com/speakeasy-sdks/test-petstore-go"
	"log"
)

func main() {
	s := testpetstorego.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->