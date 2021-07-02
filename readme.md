# MLOps Starter Pack <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [Course](#course)
- [Tools](#tools)
  - [Transpiler](#transpiler)
  - [Pipeline/Orchestrator](#pipelineorchestrator)
  - [Docker](#docker)
  - [Deployment](#deployment)
  - [Monitoring](#monitoring)

## Course

- [Machine Learning Engineering for Production (MLOps) Specialization](https://www.coursera.org/specializations/machine-learning-engineering-for-production-mlops)

## Tools

### Transpiler

Sometimes a model is transpiled to a standard model language/object which can later be read and used via other languages depending on use cases.

**Example tools**

- [ONNX](https://onnx.ai/)
- [PMML](http://dmg.org/)

### Pipeline/Orchestrator

Orchestrator should be able to parallelize and sequentialize tasks according to their dependencies. For machine learning perspective, a task can be anything related to data, e.g., ETL, data sanity check, and model training.

**Sequential tasks**

[Task A] → [Task B] → [Task C]

**Parallel tasks**

[Task A] → [Task B] → [Task C]

[Task D] → [Task E]

**Example tools**

- [Airflow](https://airflow.apache.org/)
- [Kubeflow](https://www.kubeflow.org/)
- [Dagster](https://dagster.io/)
- [Azure Data Factory](https://azure.microsoft.com/en-us/services/data-factory/)

### Docker

Docker wraps an application with its software requirements, e.g., runtime, libraries, system tools, and settings.

[Learn more here.](https://www.docker.com/resources/what-container)

### Deployment

Deployment tool is used to move your code or packages between environment and ensures that those packages are identical along the deployment process.

**Example tools**

- [Jenkins](https://www.jenkins.io/)
- [GitLab CI/CD](https://docs.gitlab.com/ee/ci/)
- [GitHub Actions](https://github.com/features/actions)

### Monitoring

After a model is deployed, there are certain things required to be monitored:

- Engineering perspective: resource utilization, latency, etc.
- Data science perspective: data (concept) drift, model metric, missing data, etc.

[See a good read on model monitoring here.](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)

**Example tools**

- [Grafana](https://grafana.com/)
