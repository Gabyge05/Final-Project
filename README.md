# defining functions

def para_circle(radius):
    para = 2 * 3.14 * radius
    print('Parameter of Circle:', para)

def para_rect(height,widht):
    para = 2 *(height + widht)
    print('Parameter of Rectangle:', para)

def para_square(side):
    para = 4 * side
    print('Parameter of Square:', para)

def ar_circle(radius):
    area = 3.14 * radius * radius
    print('Area of Circle:', area)

def ar_rect(height,widht):
    area = height * widht
    print('Area of Rectangle:', area)

def ar_square(side):
    area = side * side
    print('Area of square:', area)

print("CALCULATOR FOR GEOMETRIC SHAPES")

# Menu Options 

while True:
    print('\n MENU')
    print('1.Calculate Parameter')
    print('2.Calculate Area')
    print('3.Exit')
    option= int(input('What would you like to calculate?'))

    if option == 1:
        print('\n You selected CALCULATE PARAMETER')
        print('1.Circle')
        print('2.Rectangle')
        print('3.Square')
        print('4.Exit')
        option1 = int(input('What shape would you like to calculate the parameter?:'))

        if option1 == 1:
            radius = int(input('Enter the radius of Circle:'))
            para_circle(radius)

        elif option1 == 2:
            height = int(input('Enter the height of Rectangle:'))
            width  = int(input('Enter the widht of Rectangle:'))
            para_rect(height, width)

        elif option1 == 3:
            side = int(input('Enter the side of Square:'))
            para_square(side)

        elif option1 == 4:
            break

        else:
            print('Wrong Choice.Try again!')


    elif option == 2:
        print('\n You selected CALCULATE AREA')
        print('1.Circle')
        print('2.Rectangle')
        print('3.Square')
        print('4.Exit')
        option2= int(input('What shape would you like to calculate the area?:'))

        if option2 == 1:
            radius = int(input('Enter the radius of Circle:'))
            ar_circle(radius)

        elif option2 == 2:
            height = int(input('Enter the height of Rectangle:'))
            width = int(input('Enter the widht of Rectangle:'))
            ar_rect(height, width)

        elif option2 == 3:
            side = int(input('Enter the side of Square:'))
            ar_square(side)

        elif option2 == 4:
            break

        else:
            print('Wrong Choice.Try again!')

    elif option == 3:
        break

    else:
        print('Try again.')
            
