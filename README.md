# Temp_conversion
Convert any unit of temperature to any other unit

temp= int(input('Temp: '))
unit1=input('Celsius or Farenheit or Kelvin (C/F/K):')
unit2=input('C/F/K:')

if unit1=='C':
    if unit2=='F':
        temp= (temp*9/5)+32
        print('The temp in farenheit is:',round(temp,1),unit1)
    elif unit2== 'K':
        temp= temp+273
        print('The temp in kelvin is', round(temp,1),unit2)
    else:
        print('Invalid unit')

                

elif unit1== 'F':
    if unit2=='C':  
        temp=5/9*(temp-32) 
        print('The temp in celsius is:',round(temp,1),unit1)
    elif unit2=='K':
        temp= 5/9*(temp-32)+273
        print('The temp in Kevin is:',round(temp,1),unit2)
    else:
        print('Invalid unit')

elif unit1 == 'K':
    if unit2=='C':
        temp= temp-273
        print('The temp in celsius is:', round(temp,1),unit2)
    elif unit2=='F':
        temp= 9/5*(temp-273)+32
        print('The temp in farenheit is:', round(temp,1), unit2)
    else:
        print('Unit is invaid')
        

else:
    print('Invalid unit')