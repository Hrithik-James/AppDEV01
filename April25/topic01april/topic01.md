test_request_context() allows text to printedo the 
terminal!

```python
from flask import, url_for
app=Flask(__name__) 

@app.route('/products')
def products():
  return 'Product List' 

@app.route('/product/<int:product_id>/<string:name>') 
def product_detail(product_id,name):
  return f'Product ID: {product_id}, Name:{name}' 

with app.test_request_context():
  ##complete the test_request_context
```
