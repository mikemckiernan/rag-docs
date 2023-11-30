# NVIDIA RAG LLM Operator

## About the RAG LLM Operator

The NVIDIA Retrieval Augmented Generation (RAG) Large Language Model (LLM) Operator
enables cluster administrators to operate and manage the lifecycle of the
software components that are necessary to run RAG pipelines in Kubernetes.

## About the RAG LLM Operator Documentation

This repository contains the product documentation for the Operator.

Product documentation for the Operator is available from <FIXME>.

## Building the Documentation

1. Build the container:

   ```shell
   docker build --pull \
     --tag rag-docs:0.1.0 \
     --file Dockerfile .
   ```

1. Run the container:

   ```shell
   docker run --rm -it -v $(pwd):/work -w /work \
     rag-docs:0.1.0 \
     bash
   ```

1. Build the documentation:

   ```shell
   ./repo docs
   ```

The HTML pages are located in the `_build/docs/.../latest` directory of your repository clone.