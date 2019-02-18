# PythonBasic5 For Loops

Prerequisite => From this tutorial onwards, it is expected that you have the following extensions in your Visual Studio Code;

1)Code Runner 2)Python

If you want to know more on how to get Python on Visual Studio Code, google it.

First thing first, create a file called called whatever you want it to be called and save it as ".py". For example like this, "PythonTutorial.py". Navigate to that file and do your coding there.

================================================================================================

<h3>For Loops</h3>

Supposedly we have a <strong>list</strong> of <strong>elements</strong>. Previously we will use the example below to print out each <strong>element</strong> from the <strong>list</strong>;

        a = ["apple","orange","pineapple","banana"]
        print(a[0])
        print(a[1])
        print(a[2])
        print(a[3])

However the method above could be tedious if we want to print out a lot of <strong>elements</strong>. With that being said, we can use the <strong>for loops</strong> instead to print out all the <strong>elements</strong> within the <strong>list</strong>. Here is an example of using the <strong>for loops</strong>;

        a = ["apple","orange","pineapple","banana"]
        for element in a:
          print(element)

Running this code, will give you the same output as the previous one but cleaner in terms of codes. Okay, let's break it down on what happens here. <strong>for</strong> itself is a pre-defined function whereas <strong>element</strong> is just a <strong>variable</strong> name and <strong>in a:</strong> refers to inside of <strong>list a</strong>. The <strong>element</strong> in the <strong>print function</strong> corresponds to the <strong>variable</strong> defined after the <strong>"for"</strong> syntax. Basically, in layman's term, we can say that, "For each variable in the list a, print them separately."

Now that we understand the concept of it, we can do more things with <strong>for loops</strong>. Check out the example below;

        a = [10,20,30,40]
        result = 0

        for num in a:
          result = result + num
        print(num)

By running the code, will you get the output of <strong>100</strong>? The name variable after the <strong>for</strong> syntax is just to make things clear so that when you work on your codes, you will know what is what as well as keeping your codes clean. Another way of writing <strong>result = result + num</strong> is <strong>result += num</strong>. It will still give out the same output.

Okay, what if I want to make a <strong>list</strong> of numbers <strong>from 1 until 10</strong>? I could manually type in each number into the <strong>list</strong> OR I could use <strong>range</strong> to do it. So how does <strong>range</strong> work? Check out the example;

        a = list(range(1,11))
        print(a)

OR you can also write like;

        a = range(1,11)
        print(a)

And it will still give you the same output. In this case, the <strong>variable a</strong> will have a <strong>list</strong> of <strong>elements 1,2,3,4,5,6,7,8,9,10</strong> but not 11. This is because the <strong>range</strong>function does not take into account the last number which in this case is number 11. Therefore, the <strong>range</strong> is from 1 until 10. To make things easier, you can also call it like this;

        for i in range(1,11)
            print(i)

It will also just print the numbers from 1 - 10.

However, what if we want to print specific numbers such as the multiplication of 2's? Well for that we use the <strong>modulo operator(%)</strong>. Here is an example;

        a = range(1,11)

        for num in a:
            if num%2 ==0:
                print num

Now if we run this code, it will only print multiplications of 2's. So how does <strong>modulo</strong> work? <strong>Modulo operator</strong> will only look at remainders of a <strong>division</strong>. For example, <strong>3%2</strong> means 3 divided by 2. Now the answer is obviously 1.5 BUT if we use modulo it will only take 1 because 1 is the remainder of 3 divided by 2.

================================================================================================

Alright it is time for <strong>Exercise</strong>!.

For this exercise, I need you to create a range between 1-100. In that range, you will need to compute all <strong>multiples of 3 and 5</strong>. Once done, run the code and it should look something like " 3,5,6,9,10 ... 100 ". Multiplication of 3 and 5 should appear only <strong>once</strong> such as 15. To accomplish this exercise, you will need to use your understanding of pythons up to this point.

Good Luck and Happy Trying!