<!-- Start SDK Example Usage -->
```go
package main

import (
	"context"
	testpetstorego "github.com/speakeasy-sdks/test-petstore-go"
	"log"
	"net/http"
)

func main() {
	s := testpetstorego.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->