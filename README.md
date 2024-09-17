## Analyzing historical mining data with Amazon Bedrock

This notebook demonstrates how a large language model like Anthropic Claude can be used to analyze unstructured text found in a mine owners report from 1939 [1].

[1] [CyrusPima528.pdf](https://minedata.azgs.arizona.edu/report/cyrus). 2011-01-1062, ADMMR mining collection, Arizona Geological Survey

## Prerequisites

This notebook is designed to be run in a [Amazon SageMaker Notebook Instance](https://docs.aws.amazon.com/sagemaker/latest/dg/nbi.html). Standalone use may require installation of additional Python packages or code modifications. If you're starting a new notebook, we recommend that you create the notebook in [Amazon SageMaker Studio](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-updated.html) instead of launching a notebook instance from the Amazon SageMaker console.

Access to Amazon Bedrock foundation models isn't granted by default. See [Manage access to Amazon Bedrock foundation models](https://docs.aws.amazon.com/bedrock/latest/userguide/model-access.html) for information on how to enable access to Anthropic Claude 3 Sonnet before running these examples.

## Permissions

To use the Converse API, you call the Converse or ConverseStream operations to send messages to a model. To call Converse, you require permission for the bedrock:InvokeModel operation. To call ConverseStream, you require permission for the bedrock:InvokeModelWithResponseStream operation.

For more information see [Identity and access management for Amazon Bedrock](https://docs.aws.amazon.com/bedrock/latest/userguide/security-iam.html)

## Clean-up

Notebook instances are compute instances running the Jupyter notebook app. You are charged for the instance type you choose, based on the duration of use. Stop Notebook instances when not in use to save cost and delete instances when no longer required.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.