# 최상위 클래스 object 상속

클래스를 정의 할 때, 명시적으로 최상위 클래스인 object를 상속하기를 권장한다.

그 이유는 파이썬 버전에 따른 호환성에 있다.

파이썬 3.x 버전 부터는 클래스 생성시에 기본적으로 object 클래스를 상속하지만,

파이썬 2.x 버전은 object의 상속 유무에 따라 new-style 클래스와 old-style 클래스를 구분한다.

new-style 클래스와 old-style 클래스는 내부적으로 차이가 있고 경우에 따라 문제를 야기 할 수 있다.

따라서, 파이썬 3.x 버전으로 작업을 하더라도 2.x 버전과의 호환성을 위해서는 명시적으로 object 클래스를 상속하는 것이 좋다. 

```python
# 파이썬 2.x 버전은 object 클래스 상속 여부에 따라 new-style, old-style 클래스가 구분 된다.

# new-style
class SampleClass(object):
		pass

# old-style
class SampleClass:
		pass
```
