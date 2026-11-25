# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Shelf photographs and stock exports, checked as they arrive |
| SageMaker AI | Facing detection, gap scoring and replenishment forecasts |
| Bedrock | Plain-language refill notes for each supervisor |
| DynamoDB | Stores, aisles, alerts and the review log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
