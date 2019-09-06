#### run with container

```bash
main() {
  git clone https://github.com/jobscale/anywaychat-web.git
  cd anywaychat-web
  docker build . -t local/anywaychat:0.0.1
  docker run --name anywaychat --rm -d -p 80:80 local/anywaychat:0.0.1
  http_proxy= curl -v 127.0.0.1
} && main
```
