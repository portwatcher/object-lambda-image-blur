# S3 Object Lambda Image Blur

dead simple dynamic blurred image generator

## Features

- configurable size, gaussian blur radius
- cache to s3 automatically, blurring happens only once

## Usage

### Configure Lambda, Execution Role, Bucket Policies

Please read aws docs to do it. This is your business.

### Install Modules

```bash
npm install    # pnpm won't work if you choose to upload a zip to aws lambda
sudo apt install zip
```

### Build

Change `bucketName` in `index.js` to your source bucket

```bash
npm run build
```

### Upload

Upload `function.zip` in your `dist` folder to aws lambda