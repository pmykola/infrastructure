## infrastructure

### configure docker to log to ELK

```bash
  service1:
    image: service1
    logging:
      driver: gelf
      options:
        gelf-address: udp://logstash-host:12201
        tag: "service1"
```
