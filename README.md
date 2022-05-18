# COSC140 lab 3

## Answers to the five questions at the end of the lab description

1. from products.models import Product
>>> p1 = Product(name='stuffed shark',description="Like a shark, but stuffed",price=45.00,minimum_age_appropriate=2,maximum_age_appropriate=43)
>>> p1.price
45.0
>>> p1.name
'stuffed shark'
>>> p1.save()

2. Product.objects.all().order_by('name')

3.
>>> p2 = Product.objects.get(name="stuffed shark")
>>> p2.price = p2.price/2
>>> p2.price
'stuffed shark'
>>>Product.objects.all()

4.
>>>Product.objects.get(name='stuffed shark').delete()
(1, {'products.Product': 1})
I'm not sure if this is supposed to happen but for me stuffed shark never had id=6. This is why I called it using its name. 

5. objects = Product.objects.filter(price<10,name__icontains='stuff').append(product)

## Lab feedback

 3-4 hours
 
 * What did you think about it?  What was good?  What could be improved?

I thought this lab was great. No issues found. I will say I could never figure out why my stuffed shark never got assigned an id of 6 though. 

## Feedback

I meant to push this to github a long time ago. 

S

Everything looks great!
