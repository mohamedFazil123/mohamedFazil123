#WELCOME TO MARSHALL MIX CALCULATOR

print("******************************************")
print("***** Welcome to Marshall Mix calculation *****")
print("******************************************")

# Taking input from user
print("ENTER THE FOLLOWING DETAILS:\n")
print(" PRESS 1 -> FOR Theoretical specific gravity of the mix (Gt)\n")
print(" PRESS 2 -> FOR Bulk specific gravity of mix (Gm)\n")
print(" PRESS 3 -> FOR Air voids percent (Vv)\n")
print(" PRESS 4 -> FOR Percent volume of bitumen (Vb)\n")
print(" PRESS 5 -> FOR Voids in mineral aggregate V M A\n")
print(" PRESS 6 -> FOR Voids filled with bitumen V F B\n")
print("PRESS 7 -> TO EXIT\n")

choice = int(input())

#Substitution in formulas

#Calculation of Theoretical specific gravity of the mix (Gt)

print("Note:-- Empty Inputs Can be Enter as -> 0 \n")
if(choice==1):
    stock =int(input("Enter the Number of Stock Piles used - .(NOTE := If 3 Stock piles used Enter as '3'. --*you can Enter upto 6 Stock piles*--) \n  "))
    additives=int(input("Enter the number of additives uses. (Note := If no additives used Enter '0'. --*you can Enter upto 2 Additives*--) \n "))

    if(stock==3 and additives==0 ):
        print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=3 and additives=0 ):\n")
        W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
        W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
        W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
        W4=float(input("Enter the weight of the Filler (W4) in Grams: "))
        Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

        G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
        G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
        G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
        G4=float(input("Enter the specific gravity of the Filler (G4) : "))
        Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

        #formula
        Gt=(W1+W2+W3+W4+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(Wb/Gb))
        print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==3 and additives==1):
        print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=3 and additives=1 ):\n")
        W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
        W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
        W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
        W4=float(input("Enter the weight of the Filler (W4) in Grams: "))
        W5=float(input("Enter the weight of the Additives (W5) in Grams: "))
        Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

        G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
        G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
        G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
        G4=float(input("Enter the specific gravity of the Filler (G4) : "))
        G5=float(input("Enter the specific gravity of the Additives (G5) : "))
        Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

        #formula
        Gt=(W1+W2+W3+W4+W5+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5+G5)+(Wb/Gb))
        print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==3 and additives==2):
         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=3 and additives=2 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the Filler (W4) in Grams: "))
         W5=float(input("Enter the weight of the Additives-1 (W5) in Grams: "))
         W6=float(input("Enter the weight of the Additives-2 (W6) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the Filler (G4) : "))
         G5=float(input("Enter the specific gravity of the Additives-1 (G5) : "))
         G6=float(input("Enter the specific gravity of the Additives-2 (G6) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula
         Gt=(W1+W2+W3+W4+W5+W6+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5+G5)(W6/G6)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==4 and additives==0):
         
         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=4 and additives=0 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the Filler (W5) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the Filler (G5) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula
         Gt=(W1+W2+W3+W4+W5+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==4 and additives==1):
         
         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=4 and additives=1 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the Additives (W5) in Grams: "))
         W6=float(input("Enter the weight of the Filler (W6) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the Additives (G5) : "))
         G6=float(input("Enter the specific gravity of the Filler (G6) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula
         Gt=(W1+W2+W3+W4+W5+W6+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5+G5)+(W6/G6)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==4 and additives==2):
         
         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=4 and additives=2 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the Additives-1 (W5) in Grams: "))
         W6=float(input("Enter the weight of the Additives-2 (W6) in Grams: "))
         W7=float(input("Enter the weight of the Filler (W7) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the Additives-1 (G5) : "))
         G6=float(input("Enter the specific gravity of the Additives-2 (G6) : "))
         G7=float(input("Enter the specific gravity of the Filler (G7) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula   
         Gt=(W1+W2+W3+W4+W5+W6+W7+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(W7/G7)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==5 and additives==0):

         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=5 and additives=0 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the coarse aggregate (W5) in Grams: "))
         W6=float(input("Enter the weight of the Filler (W6) in Grams: "))  
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))  
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the coarse aggregate (G5) : "))
         G6=float(input("Enter the specific gravity of the Filler (G6) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula   
         Gt=(W1+W2+W3+W4+W5+W6+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)
    

    if(stock==5 and additives==1):

         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=5 and additives=1 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))    
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the coarse aggregate (W5) in Grams: "))
         W6=float(input("Enter the weight of the Additives-1 (W6) in Grams: "))
         W7=float(input("Enter the weight of the Filler (W7) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))  
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the coarse aggregate (G5) : "))
         G6=float(input("Enter the specific gravity of the Additives-1 (G6) : "))
         G7=float(input("Enter the specific gravity of the Filler (G7) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula   
         Gt=(W1+W2+W3+W4+W5+W6+W7+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(W7/G7)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==5 and additives==2):

         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=5 and additives=2 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))    
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the coarse aggregate (W5) in Grams: "))
         W6=float(input("Enter the weight of the Additives-1 (W6) in Grams: "))
         W7=float(input("Enter the weight of the Additives-2 (W7) in Grams: "))
         W8=float(input("Enter the weight of the Filler (W8) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))  
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the coarse aggregate (G5) : "))
         G6=float(input("Enter the specific gravity of the Additives-1 (G6) : "))
         G7=float(input("Enter the specific gravity of the Additives-2 (G7) : "))
         G8=float(input("Enter the specific gravity of the Filler (G8) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula   
         Gt=(W1+W2+W3+W4+W5+W6+W7+W8+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(W7/G7)+(W8/G8)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)
    
    if(stock==6 and additives==0):

         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=6 and additives=0 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the coarse aggregate (W5) in Grams: "))
         W6=float(input("Enter the weight of the coarse aggregate (W6) in Grams: "))
         W7=float(input("Enter the weight of the Filler (W7) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))  
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the coarse aggregate (G5) : "))
         G6=float(input("Enter the specific gravity of the coarse aggregate (G6) : "))
         G7=float(input("Enter the specific gravity of the Filler (G7) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula
         Gt=(W1+W2+W3+W4+W5+W6+W7+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(W7/G7)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)  

    if(stock==6 and additives==1):
        
         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=6 and additives=1 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the coarse aggregate (W5) in Grams: "))
         W6=float(input("Enter the weight of the coarse aggregate (W6) in Grams: "))
         W7=float(input("Enter the weight of the Additives-1 (W7) in Grams: "))
         W8=float(input("Enter the weight of the Filler (W8) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))  
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the coarse aggregate (G5) : "))
         G6=float(input("Enter the specific gravity of the coarse aggregate (G6) : "))
         G7=float(input("Enter the specific gravity of the Additives-1 (G7) : "))
         G8=float(input("Enter the specific gravity of the Filler (G8) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula
         Gt=(W1+W2+W3+W4+W5+W6+W7+W8+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(W7/G7)+(W8/G8)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)

    if(stock==6 and additives==2):

         print(" THEORETICAL SPECIFIC GRAVITY OF THE MIX(Stock piles=6 and additives=2 ):\n")
         W1=float(input("Enter the weight of the coarse aggregate (W1) in Grams: "))
         W2=float(input("Enter the weight of the coarse aggregate (W2) in Grams: "))
         W3=float(input("Enter the weight of the coarse aggregate (W3) in Grams: "))
         W4=float(input("Enter the weight of the coarse aggregate (W4) in Grams: "))
         W5=float(input("Enter the weight of the coarse aggregate (W5) in Grams: "))
         W6=float(input("Enter the weight of the coarse aggregate (W6) in Grams: "))
         W7=float(input("Enter the weight of the Additives-1 (W7) in Grams: "))
         W8=float(input("Enter the weight of the Additives-2 (W8) in Grams: "))
         W9=float(input("Enter the weight of the Filler (W9) in Grams: "))
         Wb=float(input("Enter the weight of the Bitumen(Wb) in Grams: "))

         G1=float(input("Enter the specific gravity of the coarse aggregate (G1) : "))
         G2=float(input("Enter the specific gravity of the coarse aggregate (G2) : "))  
         G3=float(input("Enter the specific gravity of the coarse aggregate (G3) : "))
         G4=float(input("Enter the specific gravity of the coarse aggregate (G4) : "))
         G5=float(input("Enter the specific gravity of the coarse aggregate (G5) : "))
         G6=float(input("Enter the specific gravity of the coarse aggregate (G6) : "))
         G7=float(input("Enter the specific gravity of the Additives-1 (G7) : "))
         G8=float(input("Enter the specific gravity of the Additives-2 (G8) : "))
         G9=float(input("Enter the specific gravity of the Filler (G9) : "))
         Gb=float(input("Enter the specific gravity of the Bitumen (Gb) : "))

         #formula
         Gt=(W1+W2+W3+W4+W5+W6+W7+W8+W9+Wb)/((W1/G1)+(W2/G2)+(W3/G3)+(W4/G4)+(W5/G5)+(W6/G6)+(W7/G7)+(W8/G8)+(W9/G9)+(Wb/Gb))
         print(" THE THEORETICAL SPECIFIC GRAVITY OF THE MIX IS: ",Gt)
    
    if(choice<=2):
         print("MINIMUM 3 STOCK PILES NEEDED  ")
    
    if(additives<=1):
         print("MAXIMUM 2 ADDITIVES ONLY ")
         
#Calculation of Bulk specific gravity of mix (Gm)

elif(choice==2):
    print(" THE BULK SPECIFIC GRAVITY OF THE MIX :\n")
    Wm=float(input("Enter the weight of the specimen in AIR in Grams : "))
    Ww=float(input("Enter the weight of the specimen in WATER in Grams: "))
    
    #formula
    Gm=Wm/(Wm-Ww)
    print(" THE BULK SPECIFIC GRAVITY OF THE MIX IS: ",Gm)
    
#Calculation of  Air voids percent (Vv)

elif(choice==3):
    print(" THE AIR VOIDS PERCENT :\n")
    Gt=float(input("Enter the value of the Theoretical specific gravity (Gt): "))
    Gm=float(input("Enter the value of Bulk specific gravity (Gm): "))
    
    #formula
    Vv=((Gt-Gm)*100)/Gt
    print(" THE AIR VOIDS PERCENT IS: ",Vv," %")
    
#Calculation of Percent volume of bitumen (Vb)

elif(choice==4):
    print(" THE PERCENT VOLUME OF BITUMEN :\n")
    Wb=float(input("Enter the weight of the bitumen in the total mix in grams (Wb): "))
    Gb=float(input("Enter the value of apparent specific gravity of bitumen (Gb): "))
    Gt=float(input("Enter the value of thereotical specific gravity (Gt): "))
    Wt=float(input("Enter the weight of the specimen in Grams: "))

    #formula
    Vb=((Wb/Gb)*(Gt/Wt))*100
    print(" THE PERCENT VOLUME OF BITUMEN IS: ",Vb," %")

#Calculation of Voids in mineral aggregate V M A

elif(choice==5):
    print(" THE VOIDS IN MINERAL AGGREGATE V M A :\n")
    vb=float(input("Enter the percent volume of bitumen (Vb): "))
    Vv=float(input("Enter the air voids percent (Vv): "))
    
    #formula
    VMA=vb+Vv
    print(" THE VOIDS IN MINERAL AGGREGATE V M A IS: ",VMA," %")

#Calculation of Voids filled with bitumen V F B

elif(choice==6):
    print(" THE VOIDS FILLED WITH BITUMEN V F B :\n")
    VMA=float(input("Enter the voids in mineral aggregate (V M A): "))
    Vb=float(input("Enter the percent volume of bitumen (Vb): "))
    
    #formula
    VFB=(Vb*100)/VMA
    print(" THE VOIDS FILLED WITH BITUMEN V F B IS: ",VFB," %")

#EXIT

elif(choice==7):
    print("THANKS FOR USING THE MARSHALL MIX CALCULATOR")
    exit

else:
    print("INVALID CHOICE")
print("\n")
print("*********************-WELCOME-************************")    
print("Design and developed by: MOHAMED FAZIL PASHA ")
print("Under the Guidance of  Dr. VINAY H.N ")
print("SIDDAGANGA INSTITUTE OF TECHNOLOGY ")
print("****************************----------***************************")

    

    
