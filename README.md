# Credstash

Docker container for the "credstash" utility.

## Usage

This command maps your $HOME/.aws directory into the container so
credstash can access your AWS API key. You can also supply your
credentials with environment variables if needed.

```
docker run -it -v $HOME/.aws:/root/.aws --rm tozny/credstash credstash list
```

