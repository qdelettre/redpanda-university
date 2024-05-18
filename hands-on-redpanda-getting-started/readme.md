Repo for the course https://university.redpanda.com/courses/hands-on-redpanda-getting-started 

---

Use [Zellij](https://zellij.dev/) to visualize multiple terminal sessions at once.

```bash
zellij -l ./.zellij/layout.kdl
```

Use [Poetry](https://python-poetry.org/) to manage dependencies and virtual environments.


Use docker-compose to start/stop Redpanda.
```bash
docker-compose up -d
docker-compose down
```

Use the alias and export the environment variable to interact with Redpanda rpk.

```python
alias rpk='docker-compose exec redpanda rpk'
export REDPANDA_BROKERS="127.0.0.1:9092"
```

kafka-python client is installed directly from git repo due to incompatibility with python 3.12 (see [#2412](https://github.com/dpkp/kafka-python/issues/2412))
