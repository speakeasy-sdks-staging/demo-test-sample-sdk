<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	demotestsamplesdk "github.com/speakeasy-sdks-staging/demo-test-sample-sdk"
	"log"
)

func main() {
	s := demotestsamplesdk.New()

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