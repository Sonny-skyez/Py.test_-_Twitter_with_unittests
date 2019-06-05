# Py.test - Twitter with unittests

Project contains simple Twitter clone script with functionalities as: writing/reading tweet, findng hashtags,
writing tweets to backend .txt file. Project uses **Given, Then, When** metodology.
Main part of this project - tests, are testing:

- initialization (2 twitter classes),
- tweeting messages,
- tweeting with/without given username and backend,
- lenght of massages < 160,
- twitter verion,
- finding all hashtags in tweets.

Py.test functionalities used in project:

- unit test parametrization,
- fixtures,
- fixtures parametrization.
- fixtures autouse in many tests,
- monkeypatch,
- test coverage with annotations,
- marking tests - skip, xfail etc.


Also in project:
- sending request to external API,
- mocking twitter functions with Monkeypatch,
- usage of Mock and MagicMock unittest methods,
- usage of conftest.py file,
- debugging with pdb and wdb (wdb.server).

## Installation

- Clone this repository to your computer using link:

```
    https://github.com/Sonny-skyez/Py.test_-_Twitter_with_unittests
```

- Use package manager [pip](https://pypi.org/project/pip/) to install required Python packages:

```
  cd to the directory where requirements.txt is located.
  activate your virtualenv.
  run: pip install -r requirements.txt in your shell.
```
## Usage

To run tests you need to run [twitter_test](https://github.com/Sonny-skyez/Py.test_-_Twitter_with_unittests/blob/master/twitter_test.py) with **py.test** command in your venv.
The result of running 53 tests will look like this:

![alt text](https://github.com/Sonny-skyez/Py.test_-_Twitter_with_unittests/blob/master/Media_files/tests_session.jpg?raw=true)

## Test coverage

This project runs 53 test on twitter.py file testing it's functionalities. It has [100% code coverage - link](https://github.com/Sonny-skyez/Py.test_-_Twitter_with_unittests/blob/master/twitter.py%2Ccover)

![alt text](https://github.com/Sonny-skyez/Py.test_-_Twitter_with_unittests/blob/master/Media_files/coverage.jpg?raw=true)

```
Note:

> class Twitter(object):
>   version = '1.0'
  
>   def __init__(self, backend=None, username = None):
>       self.backend = backend
>       self._tweets = []
>       self.username = username

The '>' symbol means, that the line of code is covered by tests.
```



## Built With

- [Pycharm](https://www.jetbrains.com/pycharm/) - Python IDE for developers
- [Python 3.7](https://www.python.org/downloads/release/python-370/) - coding language
- [Pytest](https://docs.pytest.org/en/latest/) - Python test framework
- [unittest](https://docs.python.org/3/library/unittest.html) - Python test standard framework (Mock, MagicMock methods)
- [wdb - web debugger](https://github.com/Kozea/wdb) - powerful debugging tool

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Author

**Krzysztof Brymer** - script author [GitHub profile](https://github.com/Sonny-skyez), [Linkedin profile](https://www.linkedin.com/in/krzysztof-brymer/)

## License

[MIT License](https://choosealicense.com/licenses/mit/)
