# Apache Spark application stack for Kubernetes on Wodby

Deploy Apache Spark applications on Kubernetes with Wodby.

This repository defines the Wodby stack manifests and default service
composition for Apache Spark.

<!-- wodby:generated:start -->

## Stack contract

- [Apache Spark stack on Wodby](https://wodby.com/stacks/spark)
- [Browse Wodby application stacks](https://wodby.com/stacks)
- [Wodby stack documentation](https://wodby.com/docs/2.0/stacks/)
- [Stack manifest reference](https://wodby.com/docs/2.0/stacks/template/)

## Service definitions

- [Apache Spark master service](https://github.com/wodby/service-spark)

## What's included

| Component / service | Default configuration |
| --- | --- |
| Spark master<br>`master` | required; enabled by default |
| Spark worker<br>`worker` | required; enabled by default; links: `master` → `master` |

Enabled optional services are selected by default but can be excluded when an
app is created. Disabled optional services are available but not selected by
default. Required services cannot be excluded.

## Validate the stack manifest

```bash
wodby stack validate-manifest stack.yml --org <org-id>
```

<!-- wodby:generated:end -->
