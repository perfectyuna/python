# python
def decrator_A(fn):
    print('')
    def inner_A(x):
        print('')
        fn(x)
    return inner_A

def decrator_B(fn):
    print('')
    def inner_B(x):
        print('')
        fn(x)
    return inner_B

@decrator_B
@decrator_A
def f(x):
    print('A')
