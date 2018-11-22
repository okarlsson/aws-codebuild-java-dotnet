# Codebuild image with Java and Dotnet

This is a dockerfile that runs both java 8 and dotnet.

I needed this to run a dotnet build with Sonarscanner in AWS Codebuild since sonarscanner needs Java 8 to run. The Dockerfile in this project is simply taken from the Java 8 and .net core 2.1 dockerfiles in https://github.com/aws/aws-codebuild-docker-images.

Just build this with docker build . -t image-name and upload it to ECR or Docker Hub. Or use my public Docker Hub repo at okarlsson/aws-codebuild-java-dotnet:latest.