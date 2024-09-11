# Detailed Project Description

## Project Overview
Our project aims to estimate the accurate latitude and longitude of historical locations recorded in 1858 by inverting the Napier logarithms used in their calculations. We will utilize the Semantic Scholar API to gather relevant research and develop a mathematical model to achieve this.

## Endpoints and Fields
We will primarily use the following endpoints:
1. **/graph/v1/paper/search**: To search for papers related to Napier logarithms.
2. **/graph/v1/paper/{paperId}**: To retrieve detailed information about specific papers.

The fields we will focus on include:
- `title`
- `authors`
- `abstract`
- `venue`
- `year`
- `citationCount`
- `fieldsOfStudy`

## Usage and Users
We anticipate moderate usage with approximately 100-200 requests per day. Our user base will consist of a single researcher, and potentially around 5-10 users.

## Request Structure and Efficiency
To maintain efficiency, we will:
1. **Batch Requests**: Group multiple queries into single requests where possible.
2. **Caching**: Implement a caching mechanism to store frequently accessed data and reduce redundant API calls.
3. **Rate Limiting**: Monitor and adhere to the API's rate limits to avoid overloading the service.
4. **Field Selection**: Only request necessary fields to minimize data transfer and processing time.

By structuring our requests efficiently and leveraging the Semantic Scholar API's capabilities, we aim to conduct a thorough and effective exploration of the newly discovered journals, contributing valuable insights into the study of Napier logarithms.