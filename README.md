SF19.2.3_Testing_calculator
Создайте новый проект с необходимыми директориями и файлами.

Напишите по одному позитивному тесту для каждого метода калькулятора.

В папке app в файле calculator.py содержится код тестируемого приложения.

В папке tests в файле first_tests.py содержатся тесты приложения "калькулятор".


Результат

C:\Users\Acer\AppData\Local\Programs\Python\Python310\python.exe "C:\Program Files\JetBrains\PyCharm Community Edition 2021.3.2\plugins\python-ce\helpers\pycharm\_jb_pytest_runner.py" --target First_tests.py::TestCalc
Testing started at 17:37 ...
Launching pytest with arguments First_tests.py::TestCalc --no-header --no-summary -q in C:\Users\Acer\PycharmProjects\pythonProject8\tests

============================= test session starts =============================
collecting ... collected 5 items

First_tests.py::TestCalc::test_multiply_calculate_correctly FAILED       [ 20%]
First_tests.py:7 (TestCalc.test_multiply_calculate_correctly)
10 != 7

Expected :7
Actual   :10
<Click to see difference>

self = <First_tests.TestCalc object at 0x00000207C33B3430>

    def test_multiply_calculate_correctly(self):
>       assert self.calc.multiply(self, 5, 2) == 7
E       AssertionError: assert 10 == 7
E        +  where 10 = <function Calculator.multiply at 0x00000207C089E9E0>(<First_tests.TestCalc object at 0x00000207C33B3430>, 5, 2)
E        +    where <function Calculator.multiply at 0x00000207C089E9E0> = <class 'app.calculator.Calculator'>.multiply
E        +      where <class 'app.calculator.Calculator'> = <First_tests.TestCalc object at 0x00000207C33B3430>.calc

First_tests.py:9: AssertionError
PASSED       [ 40%]PASSED    [ 60%]FAILED         [ 80%]
First_tests.py:19 (TestCalc.test_adding_calculate_correctly)
6 != 100

Expected :100
Actual   :6
<Click to see difference>

self = <First_tests.TestCalc object at 0x00000207C33B3220>

    def test_adding_calculate_correctly(self):
>       assert  self.calc.adding(self, 4, 2) == 100
E       AssertionError: assert 6 == 100
E        +  where 6 = <function Calculator.adding at 0x00000207C3DB7250>(<First_tests.TestCalc object at 0x00000207C33B3220>, 4, 2)
E        +    where <function Calculator.adding at 0x00000207C3DB7250> = <class 'app.calculator.Calculator'>.adding
E        +      where <class 'app.calculator.Calculator'> = <First_tests.TestCalc object at 0x00000207C33B3220>.calc

First_tests.py:21: AssertionError
FAILED                      [100%]
First_tests.py:22 (TestCalc.test_adding_failed)
4 != 5

Expected :5
Actual   :4
<Click to see difference>

self = <First_tests.TestCalc object at 0x00000207C33B24D0>

    def test_adding_failed(self):
>       assert self.calc.adding(self, 2, 2) == 5
E       AssertionError: assert 4 == 5
E        +  where 4 = <function Calculator.adding at 0x00000207C3DB7250>(<First_tests.TestCalc object at 0x00000207C33B24D0>, 2, 2)
E        +    where <function Calculator.adding at 0x00000207C3DB7250> = <class 'app.calculator.Calculator'>.adding
E        +      where <class 'app.calculator.Calculator'> = <First_tests.TestCalc object at 0x00000207C33B24D0>.calc

First_tests.py:24: AssertionError





First_tests.py::TestCalc::test_division_calculate_correctly 
First_tests.py::TestCalc::test_subtraction_calculate_correctly 
First_tests.py::TestCalc::test_adding_calculate_correctly 
First_tests.py::TestCalc::test_adding_failed 

========================= 3 failed, 2 passed in 0.13s =========================

Process finished with exit code 1

