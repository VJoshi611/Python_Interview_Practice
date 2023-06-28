# Collinear Point
Company : Google

Q] Given three points P1[x1,y1], P2[x2,y2], P3[x3,y3]. Check whether given three points are collinear or not. 

*Mathematical approach 1* :

Find slope of P1,P2 and P2,P3. if slope of both are equal then points are collinear.

y2 - y1 / x2-x1  =  y3 - y2 / x3-x2

i.e  (y2 - y1)(x3-x2) = (x2-x1)(y3 - y2) 


code :

- Approach 1: Using slope concept
- TC: O(1)
- SC: O(1)
  
def iscollinearPoints(x1, x2, x3, y1, y2, y3):

    if((y2 - y1)*(x3 - x2) == (y3 - y2)*(x2 - x1)):
        print("Given points are collinear")
    else:
        print("Given points are non-collinear")
  
x1, x2, x3, y1, y2, y3 = 1, 2, 3, 6, 0, 9

iscollinearPoints(x1, x2, x3, y1, y2, y3)

---------------------------------------------------------

*Approach 2* :
If Area of Triangle is 0 then points are colllinear else not

Collinearity : 1/2( x1*(y2-y3) + x2*(y3-y1) + x3*(y1-y2) ) = 0

code :

def iscollinearPoints(x1, x2, x3, y1, y2, y3):

    area = 0.5 * (x1 * (y2 - y3) + x2 * (y3 - y1) + x3 * (y1 - y2))
    if area == 0:
        print("Given points are collinear")
    else:
        print("Given points are non-collinear")
        

x1, x2, x3, y1, y2, y3 = 1, 1, 1, 6, 0, 9

iscollinearPoints(x1, x2, x3, y1, y2, y3)
