# Solving Captcha

This repository contains example notebook that shows how to apply deep learning in Amazon SageMaker.

## Introduction

This example demonstrate how to use Amazon SageMaker to build, train and deploy TensorFlow based model. In this example a deep learning model is trained to infer 4 digit numerical captcha.

## Data Generation

Data generattion script is included as `gen_captcha.py`. This uses Python's captcha library that generates audio and image CAPTCHAs. In this case only image captchas are considered. Script can be used to generate datasets based on character permutations.

### Usage

To Generate 4 digits captcha with 6 permutations

`$ python gen_captcha.py -d --npi=4 -n 6`

To Generate 4 digits captcha with 60 permutations

`$ python gen_captcha.py -d --npi=4 -n 60`

Transfer the generated datasets to Amazon S3 bucket to use it during model training.

## Next Steps  

Follow the notebook `Numeric-Captcha-SageMaker-TensorFlow` to build, train and deploy model.