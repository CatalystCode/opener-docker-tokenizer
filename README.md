# opener-docker-tokenizer

Dockerfile for OpeNER tokenizer service.

Run and test locally:

```bash
docker run -p 8080:80 cwolff/opener-docker-language-identifier
docker run -p 8081:80 cwolff/opener-docker-tokenizer

text="I went to Rome last year. It was fantastic."
text="$(curl -d "input=$text" http://localhost:8080)"
curl -d "input=$text" http://localhost:8081
```
