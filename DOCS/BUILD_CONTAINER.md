# Building Container



```bash
docker build -t  <IMAGE_NAME>:<VERSION>  .
```

### Create the image for the project
```bash
docker build -t  springboot-todo-h2-api-docker:0.1  .
```

### Check your images
```bash
docker images
```

### Run locally your image
```bash
docker run -d -p 8080:8080 --name app01 springboot-todo-h2-api-docker:0.1
```

### Go inside the container
```bash
docker exec -it app01 bash
```

### Tag your image


### upload the image





