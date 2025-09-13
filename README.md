# Python
Repo for my Python notes and practices


## Externals non-practical notes:

### Using *with* for database connections:
```Python
import sqlite3

with sqlite3.connect('example.db') as conn:
    cursor = conn.cursor()
    cursor.execute("INSERT INTO users (name) VALUES (?)", ('Alice',))
# conn.commit() is called automatically if no error; otherwise, it rolls back   
```
