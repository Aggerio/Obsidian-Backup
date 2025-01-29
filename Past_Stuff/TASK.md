
## Objective

The objective of this project/task is to evaluate your knowledge in Python, FastAPI Framework, and familiarity with Google Cloud Platform (GCP). This task will evaluate how fast you are able to learn, solve problems, and deliver the solution.

## Task Overview

- Develop two simple FastAPI endpoints and host them on Google Cloud Platform (GCP).
- You do not need to pay for anything, all services used should be free tier eligible.
  
## Task Details

### Part 1: FastAPI Endpoints with Firebase

1. **Create a FastAPI endpoint `/hello`**
    - This endpoint should print `"Hello World"`.
    - Refer to the [FastAPI Documentation](https://fastapi.tiangolo.com/).
   
2. **Create a FastAPI endpoint `/add`**
    - This endpoint should store the current date and time into Firebase Firestore.
    - **Firestore Collection Name:** `sigaram_test_collection`
    - **Document Attributes to Store:**
      - `Day of Week`: (e.g., Monday, Tuesday, etc.)
      - `Day of Month`: (e.g., 1, 2, 3, etc.)
      - `Month`: (e.g., Jan, Feb, etc.)
    - The document key should be auto-generated for uniqueness.
    - Add a timestamp of the API invocation to the Firestore database every time the `/add` API is called.
    - Reference: [Firebase Firestore Documentation](https://firebase.google.com/docs/firestore)

3. **Create a Firestore collection** called `NewsTok_test_collection` (new collection for data storage).

### Part 2: Fake Store API Integration

1. **Use the Fake Store API** to perform CRUD operations. Reference: [Fake Store API Documentation](https://fakestoreapi.com/docs)
   
2. **Create API endpoints to interact with Fake Store API**:
    - **API to list all products**: Fetch and return a list of products.
    - **API to add an item to the cart**: Create an endpoint to add one particular item to the cart.
    - **API to list all items in the cart**: Fetch and return all items currently in the cart.

### Part 3: Hosting on Google Cloud

1. **Host the FastAPI code on Google Cloud Run**:
    - Follow the guide to deploy and host FastAPI on Google Cloud Run using the free-tier services. Reference: [Secured Serverless FastAPI with Google Cloud Run](https://medium.com/codex/secured-serverless-fastapi-with-google-cloud-run-66242b916b6)
   
2. **Deploying FastAPI on Cloud Run**:
    - Deploy your FastAPI application using Google Cloud Run.
    - Make sure the setup is eligible for the Google Cloud free tier.
    - Share the Swagger URL or the API URL for testing.

3. **Share the GitHub repository** containing the source code for review.

## Reference Materials

1. [Google Cloud Python SDK Reference](https://cloud.google.com/python/docs/reference)
2. [Firebase Firestore Documentation](https://firebase.google.com/docs/firestore)
3. [FastAPI Documentation](https://fastapi.tiangolo.com/)
4. [Firebase Firestore Python Admin SDK](https://cloud.google.com/python/docs/reference/firestore/latest/admin_client)
5. [Secured Serverless FastAPI with Google Cloud Run](https://medium.com/codex/secured-serverless-fastapi-with-google-cloud-run-66242b916b6)

## Additional Notes

- Ensure all services used are within the free-tier limits on Google Cloud Platform.
- Make sure to include proper error handling and validation for the FastAPI endpoints.
- Use the Firebase Admin SDK for Python to interact with Firestore from FastAPI.
- Test the APIs locally before deploying to Google Cloud.


## TODO --> 

- [x] Check All Product endpoints
	- Read is working fine
	- Create is working
	- Update is working
- [x] Check all cart endpoints
	- Read is working
	- Update is working
	- Create is working
- [ ] Deploy to cloud run 