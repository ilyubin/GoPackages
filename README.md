# GoLang Packages

Here some GoLang packages that help perform testing.

## Packages List

* `http_client` - HTTP client with logging

```go
func Init() {
	api = http_client.Init(viper.GetString("httpbin.base_url"))
}

func GetGet() (out model.GetResponse) {
	api.Get("/get", http.StatusOK, &out)
	return
}

func PostPost(in model.PostRequest) (out model.PostResponse) {
	api.Post("/post", in, http.StatusOK, &out)
	return
}
```

* `extensions` - some extensions for GoLang

## Ask

[igor.lyubin](https://github.com/ilyubin)
