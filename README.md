# sw-architecture-styles
Software Architecture Design and styles

## Table of Contents

1. Microservices 

2. [Serverless](serveless.md) 

3. [Containers and Orchestration](Containers-and-orchestration.md) 

4. GraphQL 

## Overview

[Architecture Styles](https://docs.microsoft.com/en-us/azure/architecture/guide/architecture-styles/) Microsoft

## Microservices 

[Microservices - Martin fowler and James Lewis](https://martinfowler.com/articles/microservices.html)

[Microservices Pattern by chris richardson](https://microservices.io/)

[Evolution of scalale Microservices - ](https://www.oreilly.com/ideas/the-evolution-of-scalable-microservices)
From building microliths to designing reactive microsystems. By Jonas Bonér June 15, 2017. O'Reilly

[Designing Event First Microservices - Lightbend (InfoQ Presentation)](https://www.infoq.com/presentations/microservices-events-first-design) 

![](https://docs.microsoft.com/en-us/dotnet/standard/serverless-architecture/media/microservices-architecture.png)

## Multi-Tenant 

![](https://docs.microsoft.com/en-us/azure/sql-database/media/saas-tenancy-welcome-wingtip-tickets-app/three-tenancy-patterns.png)

## Logging

### Structured in JSON Format

{ "eventVersion": "1.0",
"userIdentity": {
    "type": "IAMUser",
    "principalId": "EX_PRINCIPAL_ID",
    "arn": "arn: aws: iam: : 123456789012: user/Alice",
    "accessKeyId": "EXAMPLE_KEY_ID",
    "accountId": "123456789012",
    "userName": "Alice"
},
"eventTime": "2014-03-06T21: 22: 54Z",
"eventSource": "ec2.amazonaws.com",
"eventName": "StartInstances",
"awsRegion": "us-east-2",
"sourceIPAddress": "205.251.233.176",
"userAgent": "ec2-api-tools1.6.12.2",
"requestParameters": {
    "instancesSet": {
        "items": [
            {
                "instanceId": "i-abcde123"
            }
        ]
    }
},
"responseElements": {
    "instancesSet": {
        "items": [
            {
                "instanceId": "i-abcde123",
                "currentState": {
                    "code": 0,
                    "name": "pending"
                },
                "previousState": {
                    "code": 80,
                    "name": "stopped"
                }
            }
        ]
    }
}

