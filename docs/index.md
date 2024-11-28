# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## GO Code

```go
// readFile reads the content of a file and returns it as a string
func readFile(filePath string) (string, error) {
 // Read the file contents into a byte slice
 data, is_error := os.ReadFile(filePath)
 if is_error != nil {
  return "", fmt.Errorf("could not read file %s: %v", filePath, is_error)
 }

 // Convert the byte slice to a string and return it
 return string(data), nil
}
```
