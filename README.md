# Cinema API
Service for cinema management written on DRF and used docker.  
As you can see, here is allowed endpoints for cinema:
![cinema allowed endpoints](https://monosnap.com/file/IHwkRo1dReC6bMMGdRR88NfhM4m0Qb)
And allowed endpoints for user:
![users allowed endpoints](https://monosnap.com/file/L4yFgddMhcDSLzA0ERz5r2AxrxMtEY)
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
