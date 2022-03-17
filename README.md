# fastAPI backend-data-api-v2

This is the data access server for personicle.

To run this server:

- Add ```config.ini ``` in project root folder.
- ``` pip install -r requirements.txt ```
- Run the server: ``` uvicorn --port 8000 --host 127.0.0.1 main:app --reload ```

### Endpoints

#### /request
- Endpoint for datastreams. 
- parameters: user_id, datatype, startTime, endTime, source (optional)
- headers: Authorization

#### /request/events
- Endpoint for events. 
- parameters: user_id, startTime, endTime, source (optional), event_type (optional)
- headers: Authorization

