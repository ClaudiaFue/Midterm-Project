# Midterm-Project
This is for the 1000 INFOTC Class

## This is the MidTerm Project
**Introduction:** 
> My name is Claudia Fuentes but my full name goes as Claudia Y. S. Fuentes

## A little bit about me

**Personal Life:** 
> I live with my mom and dad and my little sister. I also have an older sister who is married and with a child. My family is actually really big if you count all of the relatives from the other states like:
* Texas
* Tennessee
* Virginia
* Maryland
>Its also possible that there are more _unknown relatives_ as well because I only know some relatives from Texas and from Tennessee.

## **Pets**
> For pets I have in total 6 dogs and 1 guinea pig.  
> There are 3 female dogs and 3 male dogs and the guinea pig is a female as well. 
> Their names are:
* [Fee Fee](https://s3.amazonaws.com/cdn-origin-etr.akc.org/wp-content/uploads/2017/11/16105011/English-Cocker-Spaniel-Slide03.jpg)
* [Justin](https://imagesvc.meredithcorp.io/v3/mm/image?url=https%3A%2F%2Fstatic.onecms.io%2Fwp-content%2Fuploads%2Fsites%2F47%2F2021%2F03%2F09%2Fchihuahua-laying-down-wooden-floor-1675701502-2000.jpg)
* Luna
* Jesse(_male_)
* Mar
* Blue
* LeLe(_Guinea Pig_)
 ##### > This is an image of what Lele looks like but her paws are the only parts where she has the color white
![Black Guinea Pig](https://petsvills.com/wp-content/uploads/2020/08/male-black-guinea-pig-names-a.webp)
 


# Education
> Currently I am a freshman in the _[University of Missouri-Columbia](https://missouri.edu)_ but I am studying to earn a **Bachelors Degree** in Information Technology with the pathway of Engineering.
> I have graduated from _[Van Horn High School](https://sites.isdschools.org/vanhorn)_ on May 2021 in **Independence,MO**

## Code Projects
> This is a code made as a challenge in one of my INFOTC Classes in College
### What it does is to calculate the _Surface Area_ of a cylinder and also can calculate how much paint is needed to cover the cylinder.

 
 from math import pi
 
 import math
 
 #Surface area is2(pi)rh + 2(pi)r^2


def get_radius():
    
    while True:
        try:
            radius = float(input("Enter the Radius "))
            if (radius < 0):
                print("No Negative numbers")
                continue
        except ValueError:
                print("Only Numerical Values are allowed.")
        else:
            break
    return radius


def get_height():
    
    while True:
        try:
            height = float(input("Enter the Height "))
            if (height < 0):
                print("No Negative Numbers")
                continue
        except ValueError:
                print("Only Numerical Values are allowed.")
        else:
            break
    return height

def get_pint():
    
    while True:
        try:
            pint = float(input("What is the cost of Pints? "))
            if(pint < 0):
                print("No Negative Numbers")
                continue
        except ValueError:
            print("Only Numerical Values are allowed.")
        else:
            break
    return pint


def calculate_cylinder_sa(radius, height):
    
    sa = 2 * pi * radius * height + 2 * pi * radius ** 2
    return sa

def pint_total(sa):
    
    p = math.ceil(sa / 50)
    return p

def pint_report(p):
    
    print("Total Pints is ",math.ceil(p))

def pint_cost(pint,p):
    
    cost = p * pint
    print("The Cost will be $",format(cost,",.2f" ))

def generate_report(radius, height, sa):
    
    print("A Cylinder with a radius of ",radius, "and height of ",height,"has a surface area of ",sa)

def main():
    
    print("Welcome to the Cylinder Coatings Estimator.")
    print(" ")
    do_calculation = True
    while (do_calculation):
        radius = get_radius()
        height = get_height()
        pint = get_pint()
        sa = calculate_cylinder_sa(radius, height)
        generate_report(radius, height, sa)
        p = pint_total(sa)
        pint_report(p)
        p= pint_cost(pint,p)
        another_calculation = input("Do you want to continue? (Y/N): "
                                    )
        if (another_calculation != "Y"):
            do_calculation = False
            break
main()


# This is where the other markdown pages will be.
>There will be random items here and there but they will have all requirements.
* [1st page](https://github.com/ClaudiaFue/hello-world.git)
* [2nd page](https://github.com/ClaudiaFue/Interests.git)
* [3rd page](https://github.com/ClaudiaFue/Family-History.git)
* [4th page](https://github.com/ClaudiaFue/Work-Stuff.git)
> I do not know if this page counts as 1 or not
