# aws-resource-auditor-v2.3

## Overview
`aws-resource-auditor-v2.3` is a tool designed to audit AWS resources across multiple regions and services. It generates detailed reports in JSON and Excel formats.

## Features
- Audits multiple AWS services including EC2, RDS, VPC, IAM, S3, Lambda, DynamoDB, and Bedrock.
- Generates comprehensive reports in JSON and Excel formats.
- Supports multi-threaded auditing for faster results.

## Prerequisites
- Python 3.6+
- AWS credentials configured (e.g., via `aws configure`)

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/MatthewNewsum/aws-resource-audit-v2.3.git
    cd aws-resource-auditor-v2
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage
1. Run the auditor:
    ```sh
    python main.py --regions all --services all --output-dir results
    ```

    - `--regions`: Comma-separated list of regions or "all" to audit all available regions.
    - `--services`: Comma-separated list of services to audit or "all" to audit all supported services.
    - `--output-dir`: Directory to save the output reports.

2. Example:
    ```sh
    python main.py --regions us-east-1,us-west-2 --services ec2,s3 --output-dir results
    ```

## Output
- JSON report: [results/aws_inventory_<timestamp>.json](http://_vscodecontentref_/1)
- Excel report: [results/aws_inventory_<timestamp>.xlsx](http://_vscodecontentref_/2)

## Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License
This project is licensed under the MIT License.