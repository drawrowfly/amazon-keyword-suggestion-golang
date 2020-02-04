## My First App In Go

# Amazon Keyword Suggestion Tool
From 1 keyword you can get up to hundred or even thousands **Unique and Relevant Keywords** with a **Number of Active Products** per each keyword and ready to be used on Amazon.

KeyWords are collected from Amazon Web API

Result will be saved to a csv file

```go
go run main.go -keyword "iphone case" -limit 1000
```

## CSV Example
![Demo](https://i.imgur.com/OwCLSev.png)

## Result in CLI
```
Amazon KeyWord Collector Started. Collect 1000 relevant keywords for the keyword 'iphone case' 
Result: 10 keywords related to the keyword 'iphone case' were saved to the 'iphone case.csv' file 
```

# Commands
```
  -keyword string
        keyword to use (default "iphone")
  -limit int
        number of keywords to collect (default 100)
  -concurency int
        the number of goroutines that are allowed to run concurrently (default 2)
```