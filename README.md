# Calculator
#From Dumb calculator to ...

    print("사칙연산 계산기 Ver.1")
    print("="*20)
    count=int(input("연산하실 수의 개수를 말씀해주세요.:"))
    if count <= 1:
    print("다시 시도해주세요.")
    else:
    nums=[]
    for i in range(count):
        reqnums=float(input("숫자를 계산할 순서에 맞게 입력해주세요: "))
        nums.append(reqnums)
    print(nums)
    print("1. 덧셈 / 2. 뺄셈 / 3. 곱셈 / 4. 나눗셈")
    run=int(input("원하시는 연산에 해당하는 번호를 입력해주세요.:"))

    if run == 1:
       print(sum(nums))

    elif run == 2:
        def minus(nums):
            zero=0
            for n in nums:
                zero -= n
                mans = zero + (nums[0] * 2)
            return mans
        print(minus(nums))

    elif run == 3:
        def multiply(nums):
            one = 1
            for k in nums:
                if k == 0:
                    return(0)
                one *= k
            return one
        print(multiply(nums))

    elif run == 4:
        def divide(nums):
            done = 1
            for m in nums:
                done /= m
                dans = done * (nums[0] * nums[0])
            return dans
        print(divide(nums))
    print("="*20)
    print("이용해주셔서 감사합니다!")



