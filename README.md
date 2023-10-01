[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


# Weather Whisper - AWS Edition

Weather Whisper is a web-based application designed to provide users with real-time weather information. This AWS Edition showcases the full migration and optimization of the application within the AWS Cloud.

## Features

- Fetch real-time weather data for any city.
- Intuitive UI built with HTML, CSS, and JavaScript.
- Serverless backend leveraging AWS Lambda functions.
- Secure API calls using AWS API Gateway.
- Fast content delivery using Amazon CloudFront.

# AWS Services Utilized

- Amazon S3: Hosts the static website content.
- AWS Lambda: Powers the serverless backend to fetch weather data.
- Amazon API Gateway: Manages and secures API calls to the Lambda functions.
- Amazon CloudFront: Provides a fast content delivery network (CDN) for distributing the web app globally.
- Amazon Route 53: Offers domain registration and DNS routing to the CloudFront distribution.
- AWS Certificate Manager: Ensures secure HTTPS connections via SSL certificates.

## Challenges & Solutions

- CORS Issues: Encountered CORS restrictions when making cross-origin requests. Solved by setting appropriate CORS headers in both the Lambda response and the frontend JavaScript.
- CloudFront Caching: Recognized that CloudFront was caching old versions of files, leading to outdated content being served. This was addressed by using cache invalidations.
- Lambda Dependencies: Faced issues with missing dependencies in Lambda. Ensured Axios, a crucial HTTP client, was included in the deployment package.

## Deployment

The application is hosted using Amazon S3 and distributed via Amazon CloudFront, ensuring users from around the globe can access the app with low latency.

## Screenshots


## Future Enhancements
- Expand weather data to include forecasts, humidity, wind speed, and more.
- Implement user accounts for personalized weather dashboards.
- Integrate more advanced visualization tools to show weather patterns/trends.
