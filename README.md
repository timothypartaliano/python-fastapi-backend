# python-fastapi-backend
Simple Backend App using Python &amp; FastAPI

</br>

## Installation
1. Clone this repository
```bash
 git clone https://github.com/timothypartaliano/python-fastapi-backend.git
```

2. Get all dependencies
```bash
 pip install fastapi
 pip install uvicorn
```

3. Run the application
```bash
 uvicorn main:app --reload
```

4. Add items
```bash
 curl -X POST -H "Content-Type: application/json" 'http://127.0.0.1:8000/items?item=<item>'
 exp: curl -X POST -H "Content-Type: application/json" 'http://127.0.0.1:8000/items?item=mango'
```

5. Get items
```bash
 curl -X GET http://127.0.0.1:8000/items/<index>
 exp: curl -X GET http://127.0.0.1:8000/items/0
```

6. Get items with limit
```bash
 curl -X GET 'http://127.0.0.1:8000/items?limit=<limit>'
 exp: curl -X GET http://127.0.0.1:8000/items?limit=3'

 curl -X GET 'http://127.0.0.1:8000/items
```