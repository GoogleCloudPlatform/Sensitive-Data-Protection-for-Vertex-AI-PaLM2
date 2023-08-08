# Sensitive Data Protection (Cloud DLP) for Vertex AI Generative Models (PaLM2)

### Protecting Gen AI Applications from Data Leakage
Large language models (LLMs) are deep learning models trained on massive datasets of text. LLMs can translate language, summarize text, generate creative writing, generate code, power chatbots and virtual assistants, and complement search engines and recommendation systems.


When incorporating your own data into generative AI applications especially via [Model Tuning](https://cloud.google.com/vertex-ai/docs/generative-ai/models/tune-models) it's possible to return a prediction with data from your dataset. In this case many organizations may want to filter LLM responses for sensitive data.


By using Sensitive Data Protection(Cloud DLP) we can identify and take corrective action on sensitive data within LLM responses in real time.


### Using Sensitive Data Protection(Cloud DLP) to filter LLM Responses

[Sensitive Data Protection(Cloud DLP)](https://cloud.google.com/dlp) is a fully managed service designed to discover, classify, and protect your sensitive data, where it resides from databases, text-based content, or even images. It uses a variety of methods to identify sensitive data, including regular expressions, dictionaries, and contextual elements. Once sensitive data is identified, Sensitive Data Protection(Cloud DLP) can take several actions to either classify it, mask it, encrypt it or even delete it.


Sensitive Data Protection(Cloud DLP) can be accessed via Cloud Console and used to scan data within Cloud Storage, BigQuery and other Google Cloud services. The following notebook demonstrates using it through the SDK to incorporate Sensitive Data Protection(Cloud DLP) capabilities directly into you Generative AI enabled applications

## Setting up your Google Cloud project

You will need a Google Cloud project to use this project.

1. [Select or create a Google Cloud project](https://console.cloud.google.com/cloud-resource-manager). When you first create an account, you get a $300 free credit towards your compute/storage costs.

2. [Make sure that billing is enabled for your project](https://cloud.google.com/billing/docs/how-to/modify-project).

3. [Enable the Vertex AI API](https://console.cloud.google.com/flows/enableapi?apiid=aiplatform.googleapis.com).

## Setting up your Python or Jupyter environment

Please see the README in the [setup-env](https://github.com/GoogleCloudPlatform/generative-ai/tree/main/setup-env) folder for information on using Colab notebooks and Vertex AI Workbench.

## Google Generative AI Resources

Check out a list of [Google Generative AI Resources](RESOURCES.md) like official product pages, documentation, videos, courses and more.

## Contributing

Contributions welcome! See the [Contributing Guide](CONTRIBUTING.md).

## Getting help

Please use the [issues page](https://github.com/GoogleCloudPlatform/Sensitive-Data-Protection-for-Vertex-AI-and-PaLM2/issues) to provide feedback or submit a bug report.

## Disclaimer

This repository itself is not an officially supported Google product. The code in this repository is for demonstrative purposes only.