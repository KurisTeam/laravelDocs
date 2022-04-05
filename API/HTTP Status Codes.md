## Extension VS Code Install

| Code | HTTP Status Codes and the Response Format                                                          |
| ---- | -------------------------------------------------------------------------------------------------- |
| 200  | 200: OK. The standard success code and default option.                                             |
| 204  | 204: No content. When an action was executed successfully, but there is no content to return.      |
| 201  | 201: Object created. Useful for the store actions.                                                 |
| 206  | 206: Partial content. Useful when you have to return a paginated list of resources.                |
| 400  | 400: Bad request. The standard option for requests that fail to pass validation.                   |
| 401  | 401: Unauthorized. The user needs to be authenticated.                                             |
| 403  | 403: Forbidden. The user is authenticated, but does not have the permissions to perform an action. |
| 404  | 404: Not found. This will be returned automatically by Laravel when the resource is not found.     |
| 500  | 500: Internal server error. Ideally you're not going to be explicitly returning this.              |
| 503  | 503: Service unavailable. Pretty self explanatory.                                                 |
