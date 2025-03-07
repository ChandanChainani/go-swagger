# swagger:ignore

## Syntax:

```
swagger:ignore
```

### Example 1: Marks a struct as explicitly ignore from the Swagger spec output

```
//swagger: ignore
type Patient struct {
    // example: John Doe
    name        string  `json:"name"`
    // example: 27
    age         int     `json:"age""`
    // example: New York
    city        string  `json:"city"`
    // example: 1234567890
    phone       string  `json:"phone"`
    // example: 1A2B3C
    uniqueId    string  `json:"unique_id"`
}
```

### Example 2: Exclude a specific field from swagger spec output

```
//swagger: model Person
type Person struct {
    // example: John Doe
    name        string  `json:"name"`
    // example: 27
    age         int     `json:"age""`
    // example: New York
    city        string  `json:"city"`
    // example: 1234567890
    phone       string  `json:"phone"`
    // example: 1A2B3C
    // swagger: ignore
    uniqueId    string  `json:"unique_id"`
}
```
