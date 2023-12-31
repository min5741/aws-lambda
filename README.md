# aws-lambda-image-resize
AWS Lambda function to resize images present in AWS S3

# Prerequisites
* [AWS CLI](https://aws.amazon.com/cli/)
* [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)

# Setup
```
git clone https://github.com/mina178/aws-lambda-image-resize.git
cd aws-lambda-image-resize
npm install
npm remove --save sharp
npm install --save --arch=x64 --platform=linux --target=8.10.0 sharp
```

# Run
Set the input parameters in test-data/resize_image.json and run
```
sam local invoke ResizeImageFunction  --event test-data/resize_image.json 
```

# Examples
* Original Image - examples/images/test.JPG (2.9 MB, 4000x3000)
* Resized Image - examples/images-compressed/test.JPG (48 KB, 800x600)

