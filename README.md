# pypi
Reminder of how we create a python package 


## Creating a Python Package

Tutorial:
- https://youtu.be/9Ii34WheBOA?t=457


This is my first Python package. Here’s how to build one.

### Steps to Create a Pip Package:

1. Install or upgrade the build tool:  
   ```bash
   pip install --upgrade build
   ```

2. Navigate to your project’s root directory:  
   ```bash
   cd "GIT_PROJECT_ROOT"
   ```

3. Build the package:  
   ```bash
   python -m build
   ```

4. A `.whl` file will be created. You can install it using pip:  
   ```bash
   pip install iid-2025.1.8-py3-none-any.whl
   ```

### Example Workflow:

```bash
python -m build
pip uninstall iid -y
python -m build
pip install dist/iid42-2025.1.8-py3-none-any.whl
python
```



### Example Usage:

```python
import iid
iid.say_hello()
```




```
pip install --upgrade twine
python -m twine upload dist/*

```

Use https://test.pypi.org for training.  
https://youtu.be/9Ii34WheBOA?t=699  



USER_PATH/.pypirc  
```
[distutils]
index-servers =
    pypi
    
[pypi]
username = __token__
password = pypi-AgEIc...
```

