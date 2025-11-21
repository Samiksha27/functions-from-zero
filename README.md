# functions-from-zero
Coursera training

$ touch Hello.py
$ python Hello.py
$ touch Makefile
$ touch requirements.txt
$ touch test_Hello.py


$ make lint
pylint --disable=R,C *.py
************* Module Hello
Hello.py:13:26: W0631: Using possibly undefined loop variable 'key' (undefined-loop-variable)

-----------------------------------
Your code has been rated at 8.75/10

make: *** [Makefile:12: lint] Error 4

$ make lint
pylint --disable=R,C *.py
************* Module Hello
Hello.py:13:26: W0631: Using possibly undefined loop variable 'key' (undefined-loop-variable)
Hello.py:17:0: W0127: Assigning the same variable 'my_dict' to itself (self-assigning-variable)

------------------------------------------------------------------
Your code has been rated at 7.78/10 (previous run: 8.75/10, -0.97)



@Samiksha27 ➜ /workspaces/functions-from-zero (main) $ make test
python -m pytest -vv test_Hello.py
============================================= test session starts ==============================================
platform linux -- Python 3.12.1, pytest-9.0.1, pluggy-1.6.0 -- /home/codespace/.python/current/bin/python
cachedir: .pytest_cache
rootdir: /workspaces/functions-from-zero
plugins: anyio-4.11.0
collected 1 item                                                                                               

test_Hello.py::test_add PASSED   
