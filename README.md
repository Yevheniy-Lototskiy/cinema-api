# Cinema API
Service for cinema management written on DRF and used docker.

### Installation
Before installing the project, you need to install the PostgreSQL and create a database in it.
You also need to install the Docker to be able to use it.  
When it is done, run next commands:

```git clone https://github.com/Yevheniy-Lototskiy/cinema-api.git```  
```cd cinema-api```  
```python -m venv venv```  
```source venv/bin/activate``` (macOS or Linux)  
```venv\Scripts\activate``` (Windows)  
```pip install -r requirements.txt```  
```set POSTGRES_HOST=<your db host>```  
```set POSTGRES_DB=<your db name>```  
```set POSTGRES_USER=<your db user```  
```set POSTGRES_PASSWORD=<your db password```  
```python manage.py migrate```  
```python manage.py runserver```  

### Run with docker
```docker-compose build```  
```docker-compose up```

### Getting access
- Create user via ```localhols:8000/api/user/register/```
- get access token via ```localhost:8000/api/user/token/```

### Features
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres and actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

### Screenshots
As you can see, here is allowed endpoints for cinema:
![cinema allowed endpoints](media/screenshots/cinema_allowed_endpoints.png)
And allowed endpoints for user:
![users allowed endpoints](media/screenshots/users_allowed_endpoints.png)
