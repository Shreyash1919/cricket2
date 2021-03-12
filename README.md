import random

Format_choose=input("Choose you format(TEST/ODI/T20):")
print("--------------------------------")

print("Team 2 will do the call")

print("--------------------------------")

d={'India':'IND','England':'ENG','Australia':'AUS','Blackcaps':'NZ','South_Africa':'SA','West_Indies':'WI','Sri_Lanka':'SL'}
for key,value in d.items():
    print(key,':',value)

print("--------------------------------")

x=input("Choose your Team 1 :")
y=input("Choose your Team 2 :")

x_1=0
y_1=0

print("--------------------------------")

print("Get ready for",x,"VS",y,"match")

print("--------------------------------")

Toss = str(input("Team 2 call's the toss(H/T):"))

i = random.randint(1,2)
H=""
T=""

if i==1:
    if Toss == "H":
        Bat_Ball = str(input("Team 2 has won the toss and chose to :"))
        y_1 = y_1 + 1
    else:
        Bat_Ball = str(input("Team 1 has won the toss and chose to :"))
        x_1 = x_1 + 1
if i==2:
    if Toss == "T":
        Bat_Ball = str(input("Team 2 has won the toss and chose to :"))        
        y_1 = y_1 + 1
    else:
        Bat_Ball = str(input("Team 1 has won the toss and chose to :"))
        x_1 = x_1 + 1


print("--------------------------------")

if y_1 == 1:
    if Bat_Ball == "Bat" or Bat_Ball == "BAT" or Bat_Ball == "bat":
        print(y)
        print("--------------------------------")#batting order of y 1st then x
        print("Player name" ,end="\t")
        print("Score" ,end="\t")
        print("No of balls played")

        
        if y == "IND":
            wick = 0
            print("Rohit Sharma",end="\t")
            a = 0
            a_1 = 0
            if Format_choose == "T20":
                while a_1 < 120:
                    a1 = random.randint(0,6)
                    A1 = random.randint(0,1)
                    if a1 == 5 and A1 == 0:
                        a_1 += 1
                        wick += 1
                        break
                    if a1 != 5:
                        if a1 == 3:
                            a = a + 2
                        else:
                            a = a + a1
                    a_1 += 1
            elif Format_choose =="ODI":
                 while a_1 < 300:
                     a1 = random.randint(0,6)
                     A1 = random.randint(0,4)
                     if a1 == 0 and A1 == 0:
                         a_1 += 1
                         wick += 1
                         break
                     a = a + a1
                     a_1 += 1
            elif Format_choose == "TEST":
                while True:
                     a1 = random.randint(0,6)
                     A1 = random.randint(0,4)
                     if a1 == 0 and A1 == 0:
                         a_1 += 1
                         wick += 1
                         break
                     a = a + a1
                     a_1 += 1
            print(a,end="\t")
    
            print((a_1))

                


            print("KL Rahul",end="\t")
            b = 0
            b_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 ) < 120:
                    b1 = random.randint(0,6)
                    
                    B1 = random.randint(0,1)
                    if b1 == 5 and B1 == 0:
                        b_1 += 1
                        wick += 1
                        break
                    if b1 != 5:
                        if b1 == 3:
                            b = b + 2
                        else:
                            b = b + b1
                    b_1 += 1
            elif Format_choose =="ODI":
                 while (a_1 + b_1 ) < 300:
                     b1 = random.randint(0,6)
                     B1 = random.randint(0,4)
                     if b1 == 0 and B1 == 0:
                         b_1 += 1
                         wick += 1
                         break
                     b = b + b1
                     b_1 += 1
            elif Format_choose == "TEST":
                while True:
                     b1 = random.randint(0,6)
                     B1 = random.randint(0,4)
                     if b1 == 0 and B1 == 0:
                         b_1 += 1
                         wick += 1
                         break
                     b = b + b1
                     b_1 += 1
            print(b,end="\t")
    
            print((b_1))


            print("Virat Kholi",end="\t")
            c = 0
            c_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 ) < 120:
                    c1 = random.randint(0,6)
                    
                    C1 = random.randint(0,1)
                    if c1 == 5 and C1 == 0:
                        c_1 += 1
                        wick += 1
                        break
                    if c1 != 5:
                        if c1 == 3:
                            c += 2
                        else:
                            c += c1
                    c_1 += 1
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 ) < 300:
                     c1 = random.randint(0,6)
                     C1 = random.randint(0,4)
                     if c1 == 0 and C1 == 0:
                         c_1 += 1
                         wick += 1
                         break
                     c = c + c1
                     c_1 += 1
            elif Format_choose == "TEST":
                while True:
                     c1 = random.randint(0,6)
                     C1 = random.randint(0,4)
                     if c1 == 0 and C1 == 0:
                         c_1 += 1
                         wick += 1
                         break
                     c = c + c1
                     c_1 += 1
            print(c,end="\t")
    
            print((c_1))


            print("Shreyas Iyer",end="\t")
            e = 0
            e_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 ) < 120:
                    e1 = random.randint(0,6)
                   
                    E1 = random.randint(0,1)
                    if e1 == 5 and E1 == 0:
                        e_1 += 1
                        wick += 1
                        break
                    if e1 != 5: 
                        if e1 == 3:
                            e += 1
                        else:
                            e += e1
                    e_1 += 1
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 + e_1 ) < 300:
                     e1 = random.randint(0,6)
                     E1 = random.randint(0,4)
                     if e1 == 0 and E1 == 0:
                         e_1 += 1
                         wick += 1
                         break
                     e += e1
                     e_1 += 1
            elif Format_choose == "TEST":
                while True:
                     e1 = random.randint(0,6)
                     E1 = random.randint(0,4)
                     if e1 == 0 and E1 == 0:
                         e_1 += 1
                         wick += 1
                         break
                     e += e1
                     e_1 += 1
            print(e,end="\t")
    
            print((e_1))


            print("Rishabh Pant",end="\t")
            f = 0
            f_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                    f1 = random.randint(0,7)
                 
                    F1 = random.randint(0,1)
                    if f1 == 5 and F1 == 0:
                        f_1 += 1
                        wick += 1
                        break
                    if f1 != 5:
                        if f1 == 3:
                            f += 2
                        else:
                            f += f1
                    f_1 += 1
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                     f1 = random.randint(0,6)
                     F1 = random.randint(0,4)
                     if f1 == 0 and F1 == 0:
                         f_1 += 1
                         wick += 1
                         break
                     f += f1
                     f_1 += 1
            elif Format_choose == "TEST":
                while True:
                     f1 = random.randint(0,6)
                     F1 = random.randint(0,4)
                     if f1 == 0 and F1 == 0:
                         f_1 += 1
                         wick += 1
                         break
                     f += f1
                     f_1 += 1
            print(f,end="\t")
    
            print((f_1))

            print("Hardik Pandya",end="\t")
            g = 0
            g_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                    g1 = random.randint(0,6)
                    G1 = random.randint(0,1)
                    
                    if g1 == 5 and G1 ==0:
                        g_1 += 1
                        wick += 1
                        break
                    if g1 != 5:
                        if g1 == 3:
                            g += 1
                        else:
                            g += g1
                    g_1 += 1
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                     g1 = random.randint(0,6)
                     G1 = random.randint(0,4)
                     if g1 == 0 and G1 == 0:
                         g_1 += 1
                         wick += 1
                         break
                     g = g + g1
                     g_1 += 1
            elif Format_choose == "TEST":
                while True:
                     g1 = random.randint(0,6)
                     G1 = random.randint(0,4)
                     if g1 == 0 and G1 == 0:
                         g_1 += 1
                         wick += 1
                         break
                     g = g + g1
                     g_1 += 1
            print(g,end="\t")
    
            print((g_1))


            print("Navdeep Saini",end="\t")
            h = 0
            h_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                    h1 = random.randint(0,6)
                    H1 = random.randint(0,1)
                   
                    if h1 == 5 and H1 == 0:
                        h_1 += 1
                        wick += 1
                        break
                    if h1 != 5:
                        if h1 == 3:
                            h += 1
                        elif h1 == 2:
                            h += 1
                        else:
                            h += h1
                    h_1 += 1
                    
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                     h1 = random.randint(0,6)
                     H1 = random.randint(0,4)
                     if h1 == 0 and H1 == 0:
                         h_1 += 1
                         wick += 1
                         break
                     h += h1
                     h_1 += 1
            elif Format_choose == "TEST":
                while True:
                     h1 = random.randint(0,6)
                     H1 = random.randint(0,4)
                     if h1 == 0 and H1 == 0:
                         h_1 += 1
                         wick += 1
                         break
                     h += h1
                     h_1 += 1
            print(h,end="\t")
    
            print((h_1))



            print("Mohd Shami",end="\t")
            j = 0
            j_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                    j1 = random.randint(0,6)
                    J1 = random.randint(0,1)
                    
                    if j1 == 5 and J1 == 0:
                        j_1 += 1
                        wick += 1
                        break
                    if j1 != 5:
                        if j1 == 3:
                            j += 0
                        elif j1 == 2:
                            j += 1
                        else:
                            j += j1
                    j_1 += 1
                
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                     j1 = random.randint(0,6)
                     J1 = random.randint(0,4)
                     if j1 == 0 and J1 == 0:
                         j_1 += 1
                         wick += 1
                         break
                     j += j1
                     j_1 += 1
            elif Format_choose == "TEST":
                while True:
                     j1 = random.randint(0,6)
                     J1 = random.randint(0,4)
                     if j1 == 0 and J1 == 0:
                         j_1 += 1
                         wick += 1
                         break
                     j += j1
                     j_1 += 1
            print(j,end="\t")
    
            print((j_1))



            print("Jaspreet Bumrah",end="\t")
            k = 0
            k_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                    k1 = random.randint(0,7)
                    K1 = random.randint(0,1)
                    
                    if k1 == 5 and K1 == 0:
                        k_1 += 1
                        wick += 1
                        break
                    if k1 != 5:
                        if k1 == 3:
                            k += 0
                        elif k1 == 2:
                            k += 0
                        elif k1 == 6:
                            k += 4
                        else:
                            k += k1
                    k_1 += 1
                   
            elif Format_choose =="ODI":
                 while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                     k1 = random.randint(0,6)
                     K1 = random.randint(0,4)
                     if k1 == 0 and K1 == 0:
                         k_1 += 1
                         wick += 1
                         break
                     k += k1
                     k_1 += 1
            elif Format_choose == "TEST":
                while True:
                     k1 = random.randint(0,6)
                     K1 = random.randint(0,4)
                     if k1 == 0 and K1 == 0:
                         k_1 += 1
                         wick += 1
                         break
                     k += k1
                     k_1 += 1
            print(k,end="\t")
    
            print((k_1))



            print("Yuzi Chahal",end="\t")
            l = 0
            l_1 = 0
            if Format_choose == "T20":
                while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                    l1 = random.randint(0,5)
                    L1 = random.randint(0,1)
                    if l1 == 5 and L1 == 0:
                        l_1 += 1
                        wick += 1
                        break
                    if l1 != 5:
                        if l1 == 3:
                            l += 0
                        elif l1 == 2:
                            l += 0
                        elif l1 == 6:
                            l += 2
                        else:
                            l += l1
                    l_1 += 1
                    
            elif Format_choose == "ODI":
                 while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                     l1 = random.randint(0,6)
                     L1 = random.randint(0,4)
                     if l1 == 0 and L1 == 0:
                         l_1 += 1
                         wick += 1
                         break
                     l = l + l1
                     l_1 += 1
            elif Format_choose == "TEST":
                while True:
                     l1 = random.randint(0,6)
                     L1 = random.randint(0,4)
                     if l1 == 0 and L1 == 0:
                         l_1 += 1
                         wick += 1
                         break
                     l = l + l1
                     l_1 += 1
            print(l,end="\t")
    
            print((l_1))

            print("--------------------------------")

            Total_score = a+b+c+e+f+g+h+j+k+l 

            Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
            abc1 = Total_balls%6
            print("Total Score :",Total_score,"/",wick,end="\n")
            print("Total overs :",(Total_balls//6+(abc1/10)))


            print("--------------------------------")

            print(x)

            print("--------------------------------")

            print("Player name" ,end="\t")
            print("Score" ,end="\t")
            print("No of balls played")
            
            if x == "ENG":
                wick = 0
                print("Jason Roy",end="\t")
                a = 0
                a_1 = 0
                if Format_choose == "T20":
                    while a_1 < 120 and a < Total_score +1:
                        a1 = random.randint(0,6)
                        A1 = random.randint(0,1)
                        if a1 == 5 and A1 == 0:
                            a_1 += 1
                            wick += 1
                            break
                        if a1 != 5:
                            if a1 == 3:
                                a = a + 2
                            else:
                                a = a + a1
                        a_1 += 1
                elif Format_choose =="ODI":
                     while a_1 < 300 and a < Total_score +1:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                elif Format_choose == "TEST":
                    while True and a < Total_score +1:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                print(a,end="\t")
        
                print((a_1))

                    


                print("J Bairstow",end="\t")
                b = 0
                b_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                        b1 = random.randint(0,6)
                        
                        B1 = random.randint(0,1)
                        if b1 == 5 and B1 == 0:
                            b_1 += 1
                            wick += 1
                            break
                        if b1 != 5:
                            if b1 == 3:
                                b = b + 2
                            else:
                                b = b + b1
                        b_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 ) < 300 and a+b < Total_score +1:
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b < Total_score+1 :
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                print(b,end="\t")
        
                print((b_1))


                print("Dawid Malan",end="\t")
                c = 0
                c_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                        c1 = random.randint(0,6)
                        
                        C1 = random.randint(0,1)
                        if c1 == 5 and C1 == 0:
                            c_1 += 1
                            wick += 1
                            break
                        if c1 != 5:
                            if c1 == 3:
                                c += 2
                            else:
                                c += c1
                        c_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c < Total_score +1:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                print(c,end="\t")
        
                print((c_1))


                print("Jos Butler",end="\t")
                e = 0
                e_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c < Total_score+1 :
                        e1 = random.randint(0,6)
                        
                        E1 = random.randint(0,1)
                        if e1 == 5 and E1 == 0:
                            e_1 += 1
                            wick += 1
                            break
                        if e1 != 5: 
                            if e1 == 3:
                                e += 1
                            else:
                                e += e1
                        e_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score +1:
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e < Total_score+1 :
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                print(e,end="\t")
        
                print((e_1))


                print("Eoin Morgan",end="\t")
                f = 0
                f_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                        f1 = random.randint(0,7)
                    
                        F1 = random.randint(0,1)
                        if f1 == 5 and F1 == 0:
                            f_1 += 1
                            wick += 1
                            break
                        if f1 != 5:
                            if f1 == 3:
                                f += 2
                            else:
                                f += f1
                        f_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f < Total_score +1:
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                print(f,end="\t")
        
                print((f_1))

                print("Ben stokes",end="\t")
                g = 0
                g_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                        g1 = random.randint(0,6)
                        G1 = random.randint(0,1)
                        
                        if g1 == 5 and G1 ==0:
                            g_1 += 1
                            wick += 1
                            break
                        if g1 != 5:
                            if g1 == 3:
                                g += 1
                            else:
                                g += g1
                        g_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g < Total_score+1 :
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                print(g,end="\t")
        
                print((g_1))


                print("Chris Wokes",end="\t")
                h = 0
                h_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score+1 :
                        h1 = random.randint(0,6)
                        H1 = random.randint(0,1)
                        
                        if h1 == 5 and H1 == 0:
                            h_1 += 1
                            wick += 1
                            break
                        if h1 != 5:
                            if h1 == 3:
                                h += 1
                            elif h1 == 2:
                                h += 1
                            else:
                                h += h1
                        h_1 += 1
                        
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score+1 :
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h < Total_score+1 :
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                print(h,end="\t")
        
                print((h_1))



                print("Moeen Ali",end="\t")
                j = 0
                j_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score +1:
                        j1 = random.randint(0,6)
                        J1 = random.randint(0,1)
                        
                        if j1 == 5 and J1 == 0:
                            j_1 += 1
                            wick += 1
                            break
                        if j1 != 5:
                            if j1 == 3:
                                j += 0
                            elif j1 == 2:
                                j += 1
                            else:
                                j += j1
                        j_1 += 1
                    
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1 :
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h+j < Total_score+1:
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                print(j,end="\t")
        
                print((j_1))



                print("Jofra Archer",end="\t")
                k = 0
                k_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                        k1 = random.randint(0,7)
                        K1 = random.randint(0,1)

                        if k1 == 5 and K1 == 0:
                            k_1 += 1
                            wick += 1
                            break
                        if k1 != 5:
                            if k1 == 3:
                                k += 0
                            elif k1 == 2:
                                k += 0
                            elif k1 == 6:
                                k += 4
                            else:
                                k += k1
                        k_1 += 1
                       
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score +1:
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h+j+k < Total_score+1 :
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                print(k,end="\t")
        
                print((k_1))



                print("Mark Wood",end="\t")
                l = 0
                l_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                        l1 = random.randint(0,5)
                        L1 = random.randint(0,1)
                        if l1 == 5 and L1 == 0:
                            l_1 += 1
                            wick += 1
                            break
                        if l1 != 5:
                            if l1 == 3:
                                l += 0
                            elif l1 == 2:
                                l += 0
                            elif l1 == 6:
                                l += 2
                            else:
                                l += l1
                        l_1 += 1
                        
                elif Format_choose == "ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                print(l,end="\t")
        
                print((l_1))

                print("--------------------------------")
              

                Total_score1 = a+b+c+e+f+g+h+j+k+l 

                Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                abc = Total_balls1%6
                print("Total Score :",Total_score1,"/",wick,end="\n")
                print("Total overs :",(Total_balls1//6+(abc/10)))


                print("--------------------------------")


            if Format_choose == "TEST":
                if Total_score>Total_score1:
                    print(y,"WON the match by",(Total_score - Total_score1),"runs")
                elif Total_score<Total_score1:
                    print(x,"WON the match by",(Total_score1 - Total_score),"runs")
                elif Total_score == Total_score1:
                    print("Match is DRAWN")
            else:
                if Total_score > Total_score1:
                    print(y,"WON the match by",(Total_score - Total_score1),"runs")
                elif Total_score < Total_score1:
                    print(x,"WON the match by",(10-wick))
            


        elif y == "ENG":
                wick = 0
                print("Jason Roy",end="\t")
                a = 0
                a_1 = 0
                if Format_choose == "T20":
                    while a_1 < 120:
                        a1 = random.randint(0,6)
                        A1 = random.randint(0,1)
                        if a1 == 5 and A1 == 0:
                            a_1 += 1
                            wick += 1
                            break
                        if a1 != 5:
                            if a1 == 3:
                                a = a + 2
                            else:
                                a = a + a1
                        a_1 += 1
                elif Format_choose =="ODI":
                     while a_1 < 300:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                print(a,end="\t")
        
                print((a_1))

                    


                print("J Bairstow",end="\t")
                b = 0
                b_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 ) < 120:
                        b1 = random.randint(0,6)
                        
                        B1 = random.randint(0,1)
                        if b1 == 5 and B1 == 0:
                            b_1 += 1
                            wick += 1
                            break
                        if b1 != 5:
                            if b1 == 3:
                                b = b + 2
                            else:
                                b = b + b1
                        b_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 ) < 300:
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                print(b,end="\t")
        
                print((b_1))


                print("Dawid Malan",end="\t")
                c = 0
                c_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 ) < 120:
                        c1 = random.randint(0,6)
                        
                        C1 = random.randint(0,1)
                        if c1 == 5 and C1 == 0:
                            c_1 += 1
                            wick += 1
                            break
                        if c1 != 5:
                            if c1 == 3:
                                c += 2
                            else:
                                c += c1
                        c_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 ) < 300:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                print(c,end="\t")
        
                print((c_1))


                print("Jos Butler",end="\t")
                e = 0
                e_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 ) < 120:
                        e1 = random.randint(0,6)
                        
                        E1 = random.randint(0,1)
                        if e1 == 5 and E1 == 0:
                            e_1 += 1
                            wick += 1
                            break
                        if e1 != 5: 
                            if e1 == 3:
                                e += 1
                            else:
                                e += e1
                        e_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 ) < 300:
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                print(e,end="\t")
        
                print((e_1))


                print("Eoin Morgan",end="\t")
                f = 0
                f_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                        f1 = random.randint(0,7)
                    
                        F1 = random.randint(0,1)
                        if f1 == 5 and F1 == 0:
                            f_1 += 1
                            wick += 1
                            break
                        if f1 != 5:
                            if f1 == 3:
                                f += 2
                            else:
                                f += f1
                        f_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                print(f,end="\t")
        
                print((f_1))

                print("Ben stokes",end="\t")
                g = 0
                g_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                        g1 = random.randint(0,6)
                        G1 = random.randint(0,1)
                        
                        if g1 == 5 and G1 ==0:
                            g_1 += 1
                            wick += 1
                            break
                        if g1 != 5:
                            if g1 == 3:
                                g += 1
                            else:
                                g += g1
                        g_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                print(g,end="\t")
        
                print((g_1))


                print("Chris Wokes",end="\t")
                h = 0
                h_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                        h1 = random.randint(0,6)
                        H1 = random.randint(0,1)
                        
                        if h1 == 5 and H1 == 0:
                            h_1 += 1
                            wick += 1
                            break
                        if h1 != 5:
                            if h1 == 3:
                                h += 1
                            elif h1 == 2:
                                h += 1
                            else:
                                h += h1
                        h_1 += 1
                        
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                print(h,end="\t")
        
                print((h_1))



                print("Moeen Ali",end="\t")
                j = 0
                j_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                        j1 = random.randint(0,6)
                        J1 = random.randint(0,1)
                        
                        if j1 == 5 and J1 == 0:
                            j_1 += 1
                            wick += 1
                            break
                        if j1 != 5:
                            if j1 == 3:
                                j += 0
                            elif j1 == 2:
                                j += 1
                            else:
                                j += j1
                        j_1 += 1
                    
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                print(j,end="\t")
        
                print((j_1))



                print("Jofra Archer",end="\t")
                k = 0
                k_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                        k1 = random.randint(0,7)
                        K1 = random.randint(0,1)

                        if k1 == 5 and K1 == 0:
                            k_1 += 1
                            wick += 1
                            break
                        if k1 != 5:
                            if k1 == 3:
                                k += 0
                            elif k1 == 2:
                                k += 0
                            elif k1 == 6:
                                k += 4
                            else:
                                k += k1
                        k_1 += 1
                       
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                print(k,end="\t")
        
                print((k_1))



                print("Mark Wood",end="\t")
                l = 0
                l_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                        l1 = random.randint(0,5)
                        L1 = random.randint(0,1)
                        if l1 == 5 and L1 == 0:
                            l_1 += 1
                            wick += 1
                            break
                        if l1 != 5:
                            if l1 == 3:
                                l += 0
                            elif l1 == 2:
                                l += 0
                            elif l1 == 6:
                                l += 2
                            else:
                                l += l1
                        l_1 += 1
                        
                elif Format_choose == "ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                print(l,end="\t")
        
                print((l_1))

                print("--------------------------------")
              

                Total_score = a+b+c+e+f+g+h+j+k+l 

                Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                abc2 = Total_balls%6 
                print("Total Score :",Total_score,"/",wick,end="\n")
                print("Total overs :",(Total_balls//6+(abc2/10)))


                print("--------------------------------")
            

                print(x)


                print("--------------------------------")

                print("Player name" ,end="\t")
                print("Score" ,end="\t")
                print("No of balls played")

                if x == "IND":
                    wick = 0
                    print("Rohit Sharma",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120 and a < Total_score +1:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300 and a < Total_score +1 :
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("KL Rahul",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 and a+b < Total_score+1 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b < Total_score +1:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Virat Kholi",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Shreyas Iyer",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c+e < Total_score+1 :
                            e1 = random.randint(0,6)
                           
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score+1 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e < Total_score +1:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Rishabh Pant",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                            f1 = random.randint(0,7)
                         
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Hardik Pandya",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g < Total_score +1:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Navdeep Saini",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score +1:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                           
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score +1:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Mohd Shami",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score+1 :
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j < Total_score+1 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jaspreet Bumrah",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)
                            
                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k < Total_score +1:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Yuzi Chahal",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score +1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                print("--------------------------------")

                Total_score1 = a+b+c+e+f+g+h+j+k+l 

                Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                abc3 = Total_balls%6
                print("Total Score :",Total_score1,"/",wick,end="\n")
                print("Total overs :",(Total_balls1//6+(abc3/10)))


                print("--------------------------------")


                if Format_choose == "TEST":
                    if Total_score>Total_score1:
                        print(y,"WON the match by",(Total_score - Total_score1),"runs")
                    elif Total_score<Total_score1:
                        print(x,"WON the match by",(Total_score1 - Total_score),"runs")
                    elif Total_score == Total_score1:
                        print("Match is DRAWN")
                else:
                    if Total_score > Total_score1:
                        print(y,"WON the match by",(Total_score - Total_score1),"runs")
                    elif Total_score < Total_score1:
                        print(x,"WON the match by",(10-wick),"WICKETS")

    elif Bat_Ball == "Bowl" or Bat_Ball == "BOWL" or Bat_Ball == "bowl":
        print(x)

        print("--------------------------------")#batting order of x 1st then y

        print("Player name" ,end="\t")
        print("Score" ,end="\t")
        print("No of balls played")

        if y == "ENG":
                    wick = 0
                    print("Rohit Sharma",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("KL Rahul",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120:
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Virat Kholi",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True :
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Shreyas Iyer",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120  :
                            e1 = random.randint(0,6)
                           
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Rishabh Pant",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 :
                            f1 = random.randint(0,7)
                         
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300  :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True  :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Hardik Pandya",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120  :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300  :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Navdeep Saini",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 :
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                           
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True  :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Mohd Shami",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 :
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jaspreet Bumrah",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120  :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)
                            
                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300  :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Yuzi Chahal",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1)<120 :
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")

                    Total_score = a+b+c+e+f+g+h+j+k+l 

                    Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc3 = Total_balls%6
                    print("Total Score :",Total_score,"/",wick,end="\n")
                    print("Total overs :",(Total_balls//6+(abc3/10)))

                    print("--------------------------------")

                    print(y)

                    print("--------------------------------")

                    print("Player name" ,end="\t")
                    print("Score" ,end="\t")
                    print("No of balls played")

                    wick = 0
                    print("Jason Roy",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120 and a < Total_score +1:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300 and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("J Bairstow",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 and a+b < Total_score +1:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b < Total_score+1 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Dawid Malan",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Jos Butler",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c < Total_score+1 :
                            e1 = random.randint(0,6)
                            
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score +1:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e < Total_score+1 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Eoin Morgan",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                            f1 = random.randint(0,7)
                        
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f < Total_score +1:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Ben stokes",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Chris Wokes",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score+1 :
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                            
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Moeen Ali",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score +1:
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j < Total_score+1:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jofra Archer",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)

                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score +1:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k < Total_score+1 :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Mark Wood",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")
                  

                    Total_score1 = a+b+c+e+f+g+h+j+k+l 

                    Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc = Total_balls1%6
                    print("Total Score :",Total_score1,"/",wick,end="\n")
                    print("Total overs :",(Total_balls1//6+(abc/10)))


                    print("--------------------------------")


                    if Format_choose == "TEST":
                        if Total_score>Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score<Total_score1:
                            print(y,"WON the match by",(Total_score1 - Total_score),"runs")
                        elif Total_score == Total_score1:
                            print("Match is DRAWN")
                    else:
                        if Total_score > Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score < Total_score1:
                            print(y,"WON the match by",(10-wick),"wickets")
                
        if y == "IND":
                    wick = 0
                    print("Jason Roy",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("J Bairstow",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120:
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Dawid Malan",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Jos Butler",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120:
                            e1 = random.randint(0,6)
                            
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Eoin Morgan",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                            f1 = random.randint(0,7)
                        
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Ben stokes",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Chris Wokes",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                            
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Moeen Ali",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jofra Archer",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)

                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Mark Wood",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")
                  

                    Total_score = a+b+c+e+f+g+h+j+k+l 

                    Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc2 = Total_balls%6 
                    print("Total Score :",Total_score,"/",wick,end="\n")
                    print("Total overs :",(Total_balls//6+(abc2/10)))


                    print("--------------------------------")
                

                    print(y)


                    print("--------------------------------")

                    print("Player name" ,end="\t")
                    print("Score" ,end="\t")
                    print("No of balls played")

                    wick = 0
                    print("Rohit Sharma",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120 and a < Total_score +1:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300 and a < Total_score +1 :
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("KL Rahul",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 and a+b < Total_score+1 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b < Total_score +1:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Virat Kholi",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Shreyas Iyer",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c+e < Total_score+1 :
                            e1 = random.randint(0,6)
                           
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score+1 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e < Total_score +1:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Rishabh Pant",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                            f1 = random.randint(0,7)
                         
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Hardik Pandya",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g < Total_score +1:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Navdeep Saini",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score +1:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                           
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score +1:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Mohd Shami",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score+1 :
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j < Total_score+1 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jaspreet Bumrah",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)
                            
                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k < Total_score +1:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Yuzi Chahal",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score +1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")

                    Total_score1 = a+b+c+e+f+g+h+j+k+l 

                    Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc3 = Total_balls%6
                    print("Total Score :",Total_score1,"/",wick,end="\n")
                    print("Total overs :",(Total_balls1//6+(abc3/10)))


                    print("--------------------------------")


                    if Format_choose == "TEST":
                        if Total_score>Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score<Total_score1:
                            print(y,"WON the match by",(Total_score1 - Total_score),"runs")
                        elif Total_score == Total_score1:
                            print("Match is DRAWN")
                    else:
                        if Total_score > Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score < Total_score1:
                            print(y,"WON the match by",(10-wick),"WICKETS")



                


            
















if x_1 == 1:
    if Bat_Ball == "Bat" or Bat_Ball == "BAT" or Bat_Ball == "bat":
        print(x)
        print("--------------------------------")#batting order of x 1st then y

        print("Player name" ,end="\t")
        print("Score" ,end="\t")
        print("No of balls played")

        if x == "IND":
                    wick = 0
                    print("Rohit Sharma",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("KL Rahul",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120:
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Virat Kholi",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Shreyas Iyer",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120:
                            e1 = random.randint(0,6)
                           
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Rishabh Pant",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                            f1 = random.randint(0,7)
                         
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Hardik Pandya",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Navdeep Saini",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                           
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Mohd Shami",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jaspreet Bumrah",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)
                            
                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Yuzi Chahal",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")

                    Total_score = a+b+c+e+f+g+h+j+k+l 

                    Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc1 = Total_balls%6
                    print("Total Score :",Total_score,"/",wick,end="\n")
                    print("Total overs :",(Total_balls//6+(abc1/10)))


                    print("--------------------------------")

                    print(y)

                    print("--------------------------------")


                    print("Player name" ,end="\t")
                    print("Score" ,end="\t")
                    print("No of balls played")


                    wick = 0
                    print("Jason Roy",end="\t")
                    a = 0
                    a_1 = 0     
                    if Format_choose == "T20":
                        while a_1 < 120 and a < Total_score +1:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300 and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("J Bairstow",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 and a+b < Total_score +1:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b < Total_score+1 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Dawid Malan",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Jos Butler",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c < Total_score+1 :
                            e1 = random.randint(0,6)
                            
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score +1:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e < Total_score+1 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Eoin Morgan",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                            f1 = random.randint(0,7)
                        
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f < Total_score +1:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Ben stokes",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Chris Wokes",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score+1 :
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                            
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Moeen Ali",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score +1:
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j < Total_score+1:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jofra Archer",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)

                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score +1:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k < Total_score+1 :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Mark Wood",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")
                  

                    Total_score1 = a+b+c+e+f+g+h+j+k+l 

                    Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc = Total_balls1%6
                    print("Total Score :",Total_score1,"/",wick,end="\n")
                    print("Total overs :",(Total_balls1//6+(abc/10)))


                    print("--------------------------------")


                    if Format_choose == "TEST":
                        if Total_score>Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score<Total_score1:
                            print(y,"WON the match by",(Total_score1 - Total_score),"runs")
                        elif Total_score == Total_score1:
                            print("Match is DRAWN")
                    else:
                        if Total_score > Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score < Total_score1:
                            print(y,"WON the match by",(10-wick),"wickets")
        elif x == "ENG":
                    wick = 0
                    print("Jason Roy",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("J Bairstow",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120:
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Dawid Malan",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Jos Butler",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120:
                            e1 = random.randint(0,6)
                            
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Eoin Morgan",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                            f1 = random.randint(0,7)
                        
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Ben stokes",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Chris Wokes",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                            
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Moeen Ali",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jofra Archer",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)

                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Mark Wood",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")
                  

                    Total_score = a+b+c+e+f+g+h+j+k+l 

                    Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc2 = Total_balls%6 
                    print("Total Score :",Total_score,"/",wick,end="\n")
                    print("Total overs :",(Total_balls//6+(abc2/10)))


                    print("--------------------------------")
                

                    print(y)


                    print("--------------------------------")

                    print("Player name" ,end="\t")
                    print("Score" ,end="\t")
                    print("No of balls played")

                    wick = 0
                    print("Rohit Sharma",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120 and a < Total_score +1:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300 and a < Total_score +1 :
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("KL Rahul",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 and a+b < Total_score+1 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b < Total_score +1:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Virat Kholi",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Shreyas Iyer",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c+e < Total_score+1 :
                            e1 = random.randint(0,6)
                           
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score+1 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e < Total_score +1:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Rishabh Pant",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                            f1 = random.randint(0,7)
                         
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Hardik Pandya",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g < Total_score +1:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Navdeep Saini",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score +1:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                           
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score +1:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Mohd Shami",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score+1 :
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j < Total_score+1 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jaspreet Bumrah",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)
                            
                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k < Total_score +1:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Yuzi Chahal",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score +1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")

                    Total_score1 = a+b+c+e+f+g+h+j+k+l 

                    Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc3 = Total_balls%6
                    print("Total Score :",Total_score1,"/",wick,end="\n")
                    print("Total overs :",(Total_balls1//6+(abc3/10)))


                    print("--------------------------------")


                    if Format_choose == "TEST":
                        if Total_score>Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score<Total_score1:
                            print(y,"WON the match by",(Total_score1 - Total_score),"runs")
                        elif Total_score == Total_score1:
                            print("Match is DRAWN")
                    else:
                        if Total_score > Total_score1:
                            print(x,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score < Total_score1:
                            print(y,"WON the match by",(10-wick),"WICKETS")




            
                

            
            




















    elif Bat_Ball == "Bowl" or Bat_Ball == "BOWL" or Bat_Ball == "bowl":
        print(y)

        print("--------------------------------")#batting order of y 1st then x

        print("Player name" ,end="\t")
        print("Score" ,end="\t")
        print("No of balls played")

        
        if y == "IND":
                wick = 0
                print("Rohit Sharma",end="\t")
                a = 0
                a_1 = 0
                if Format_choose == "T20":
                    while a_1 < 120:
                        a1 = random.randint(0,6)
                        A1 = random.randint(0,1)
                        if a1 == 5 and A1 == 0:
                            a_1 += 1
                            wick += 1
                            break
                        if a1 != 5:
                            if a1 == 3:
                                a = a + 2
                            else:
                                a = a + a1
                        a_1 += 1
                elif Format_choose =="ODI":
                     while a_1 < 300:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                print(a,end="\t")
        
                print((a_1))

                    


                print("KL Rahul",end="\t")
                b = 0
                b_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 ) < 120:
                        b1 = random.randint(0,6)
                        
                        B1 = random.randint(0,1)
                        if b1 == 5 and B1 == 0:
                            b_1 += 1
                            wick += 1
                            break
                        if b1 != 5:
                            if b1 == 3:
                                b = b + 2
                            else:
                                b = b + b1
                        b_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 ) < 300:
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                print(b,end="\t")
        
                print((b_1))


                print("Virat Kholi",end="\t")
                c = 0
                c_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 ) < 120:
                        c1 = random.randint(0,6)
                        
                        C1 = random.randint(0,1)
                        if c1 == 5 and C1 == 0:
                            c_1 += 1
                            wick += 1
                            break
                        if c1 != 5:
                            if c1 == 3:
                                c += 2
                            else:
                                c += c1
                        c_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 ) < 300:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                print(c,end="\t")
        
                print((c_1))


                print("Shreyas Iyer",end="\t")
                e = 0
                e_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 ) < 120:
                        e1 = random.randint(0,6)
                       
                        E1 = random.randint(0,1)
                        if e1 == 5 and E1 == 0:
                            e_1 += 1
                            wick += 1
                            break
                        if e1 != 5: 
                            if e1 == 3:
                                e += 1
                            else:
                                e += e1
                        e_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 ) < 300:
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                print(e,end="\t")
        
                print((e_1))


                print("Rishabh Pant",end="\t")
                f = 0
                f_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                        f1 = random.randint(0,7)
                     
                        F1 = random.randint(0,1)
                        if f1 == 5 and F1 == 0:
                            f_1 += 1
                            wick += 1
                            break
                        if f1 != 5:
                            if f1 == 3:
                                f += 2
                            else:
                                f += f1
                        f_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                print(f,end="\t")
        
                print((f_1))

                print("Hardik Pandya",end="\t")
                g = 0
                g_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                        g1 = random.randint(0,6)
                        G1 = random.randint(0,1)
                        
                        if g1 == 5 and G1 ==0:
                            g_1 += 1
                            wick += 1
                            break
                        if g1 != 5:
                            if g1 == 3:
                                g += 1
                            else:
                                g += g1
                        g_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                print(g,end="\t")
        
                print((g_1))


                print("Navdeep Saini",end="\t")
                h = 0
                h_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                        h1 = random.randint(0,6)
                        H1 = random.randint(0,1)
                       
                        if h1 == 5 and H1 == 0:
                            h_1 += 1
                            wick += 1
                            break
                        if h1 != 5:
                            if h1 == 3:
                                h += 1
                            elif h1 == 2:
                                h += 1
                            else:
                                h += h1
                        h_1 += 1
                        
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                print(h,end="\t")
        
                print((h_1))



                print("Mohd Shami",end="\t")
                j = 0
                j_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                        j1 = random.randint(0,6)
                        J1 = random.randint(0,1)
                        
                        if j1 == 5 and J1 == 0:
                            j_1 += 1
                            wick += 1
                            break
                        if j1 != 5:
                            if j1 == 3:
                                j += 0
                            elif j1 == 2:
                                j += 1
                            else:
                                j += j1
                        j_1 += 1
                    
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                print(j,end="\t")
        
                print((j_1))



                print("Jaspreet Bumrah",end="\t")
                k = 0
                k_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                        k1 = random.randint(0,7)
                        K1 = random.randint(0,1)
                        
                        if k1 == 5 and K1 == 0:
                            k_1 += 1
                            wick += 1
                            break
                        if k1 != 5:
                            if k1 == 3:
                                k += 0
                            elif k1 == 2:
                                k += 0
                            elif k1 == 6:
                                k += 4
                            else:
                                k += k1
                        k_1 += 1
                       
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                print(k,end="\t")
        
                print((k_1))



                print("Yuzi Chahal",end="\t")
                l = 0
                l_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                        l1 = random.randint(0,5)
                        L1 = random.randint(0,1)
                        if l1 == 5 and L1 == 0:
                            l_1 += 1
                            wick += 1
                            break
                        if l1 != 5:
                            if l1 == 3:
                                l += 0
                            elif l1 == 2:
                                l += 0
                            elif l1 == 6:
                                l += 2
                            else:
                                l += l1
                        l_1 += 1
                        
                elif Format_choose == "ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                elif Format_choose == "TEST":
                    while True:
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                print(l,end="\t")
        
                print((l_1))

                print("--------------------------------")

                Total_score = a+b+c+e+f+g+h+j+k+l 

                Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                abc1 = Total_balls%6
                print("Total Score :",Total_score,"/",wick,end="\n")
                print("Total overs :",(Total_balls//6+(abc1/10)))


                print("--------------------------------")

                print(x)

                print("--------------------------------")

                print("Player name" ,end="\t")
                print("Score" ,end="\t")
                print("No of balls played")            



                wick = 0
                print("Jason Roy",end="\t")
                a = 0
                a_1 = 0
                if Format_choose == "T20":
                    while a_1 < 120 and a < Total_score +1:
                        a1 = random.randint(0,6)
                        A1 = random.randint(0,1)
                        if a1 == 5 and A1 == 0:
                            a_1 += 1
                            wick += 1
                            break
                        if a1 != 5:
                            if a1 == 3:
                                a = a + 2
                            else:
                                a = a + a1
                        a_1 += 1
                elif Format_choose =="ODI":
                     while a_1 < 300 and a < Total_score +1:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                elif Format_choose == "TEST":
                    while True and a < Total_score +1:
                         a1 = random.randint(0,6)
                         A1 = random.randint(0,4)
                         if a1 == 0 and A1 == 0:
                             a_1 += 1
                             wick += 1
                             break
                         a = a + a1
                         a_1 += 1
                print(a,end="\t")
        
                print((a_1))

                    


                print("J Bairstow",end="\t")
                b = 0
                b_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                        b1 = random.randint(0,6)
                        
                        B1 = random.randint(0,1)
                        if b1 == 5 and B1 == 0:
                            b_1 += 1
                            wick += 1
                            break
                        if b1 != 5:
                            if b1 == 3:
                                b = b + 2
                            else:
                                b = b + b1
                        b_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 ) < 300 and a+b < Total_score +1:
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b < Total_score+1 :
                         b1 = random.randint(0,6)
                         B1 = random.randint(0,4)
                         if b1 == 0 and B1 == 0:
                             b_1 += 1
                             wick += 1
                             break
                         b = b + b1
                         b_1 += 1
                print(b,end="\t")
        
                print((b_1))


                print("Dawid Malan",end="\t")
                c = 0
                c_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                        c1 = random.randint(0,6)
                        
                        C1 = random.randint(0,1)
                        if c1 == 5 and C1 == 0:
                            c_1 += 1
                            wick += 1
                            break
                        if c1 != 5:
                            if c1 == 3:
                                c += 2
                            else:
                                c += c1
                        c_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c < Total_score +1:
                         c1 = random.randint(0,6)
                         C1 = random.randint(0,4)
                         if c1 == 0 and C1 == 0:
                             c_1 += 1
                             wick += 1
                             break
                         c = c + c1
                         c_1 += 1
                print(c,end="\t")
        
                print((c_1))


                print("Jos Butler",end="\t")
                e = 0
                e_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c < Total_score+1 :
                        e1 = random.randint(0,6)
                        
                        E1 = random.randint(0,1)
                        if e1 == 5 and E1 == 0:
                            e_1 += 1
                            wick += 1
                            break
                        if e1 != 5: 
                            if e1 == 3:
                                e += 1
                            else:
                                e += e1
                        e_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score +1:
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e < Total_score+1 :
                         e1 = random.randint(0,6)
                         E1 = random.randint(0,4)
                         if e1 == 0 and E1 == 0:
                             e_1 += 1
                             wick += 1
                             break
                         e += e1
                         e_1 += 1
                print(e,end="\t")
        
                print((e_1))


                print("Eoin Morgan",end="\t")
                f = 0
                f_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                        f1 = random.randint(0,7)
                    
                        F1 = random.randint(0,1)
                        if f1 == 5 and F1 == 0:
                            f_1 += 1
                            wick += 1
                            break
                        if f1 != 5:
                            if f1 == 3:
                                f += 2
                            else:
                                f += f1
                        f_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f < Total_score +1:
                         f1 = random.randint(0,6)
                         F1 = random.randint(0,4)
                         if f1 == 0 and F1 == 0:
                             f_1 += 1
                             wick += 1
                             break
                         f += f1
                         f_1 += 1
                print(f,end="\t")
        
                print((f_1))

                print("Ben stokes",end="\t")
                g = 0
                g_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                        g1 = random.randint(0,6)
                        G1 = random.randint(0,1)
                        
                        if g1 == 5 and G1 ==0:
                            g_1 += 1
                            wick += 1
                            break
                        if g1 != 5:
                            if g1 == 3:
                                g += 1
                            else:
                                g += g1
                        g_1 += 1
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g < Total_score+1 :
                         g1 = random.randint(0,6)
                         G1 = random.randint(0,4)
                         if g1 == 0 and G1 == 0:
                             g_1 += 1
                             wick += 1
                             break
                         g = g + g1
                         g_1 += 1
                print(g,end="\t")
        
                print((g_1))


                print("Chris Wokes",end="\t")
                h = 0
                h_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score+1 :
                        h1 = random.randint(0,6)
                        H1 = random.randint(0,1)
                        
                        if h1 == 5 and H1 == 0:
                            h_1 += 1
                            wick += 1
                            break
                        if h1 != 5:
                            if h1 == 3:
                                h += 1
                            elif h1 == 2:
                                h += 1
                            else:
                                h += h1
                        h_1 += 1
                        
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score+1 :
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h < Total_score+1 :
                         h1 = random.randint(0,6)
                         H1 = random.randint(0,4)
                         if h1 == 0 and H1 == 0:
                             h_1 += 1
                             wick += 1
                             break
                         h += h1
                         h_1 += 1
                print(h,end="\t")
        
                print((h_1))



                print("Moeen Ali",end="\t")
                j = 0
                j_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score +1:
                        j1 = random.randint(0,6)
                        J1 = random.randint(0,1)
                        
                        if j1 == 5 and J1 == 0:
                            j_1 += 1
                            wick += 1
                            break
                        if j1 != 5:
                            if j1 == 3:
                                j += 0
                            elif j1 == 2:
                                j += 1
                            else:
                                j += j1
                        j_1 += 1
                    
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1 :
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h+j < Total_score+1:
                         j1 = random.randint(0,6)
                         J1 = random.randint(0,4)
                         if j1 == 0 and J1 == 0:
                             j_1 += 1
                             wick += 1
                             break
                         j += j1
                         j_1 += 1
                print(j,end="\t")
        
                print((j_1))



                print("Jofra Archer",end="\t")
                k = 0
                k_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                        k1 = random.randint(0,7)
                        K1 = random.randint(0,1)

                        if k1 == 5 and K1 == 0:
                            k_1 += 1
                            wick += 1
                            break
                        if k1 != 5:
                            if k1 == 3:
                                k += 0
                            elif k1 == 2:
                                k += 0
                            elif k1 == 6:
                                k += 4
                            else:
                                k += k1
                        k_1 += 1
                       
                elif Format_choose =="ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score +1:
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h+j+k < Total_score+1 :
                         k1 = random.randint(0,6)
                         K1 = random.randint(0,4)
                         if k1 == 0 and K1 == 0:
                             k_1 += 1
                             wick += 1
                             break
                         k += k1
                         k_1 += 1
                print(k,end="\t")
        
                print((k_1))



                print("Mark Wood",end="\t")
                l = 0
                l_1 = 0
                if Format_choose == "T20":
                    while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                        l1 = random.randint(0,5)
                        L1 = random.randint(0,1)
                        if l1 == 5 and L1 == 0:
                            l_1 += 1
                            wick += 1
                            break
                        if l1 != 5:
                            if l1 == 3:
                                l += 0
                            elif l1 == 2:
                                l += 0
                            elif l1 == 6:
                                l += 2
                            else:
                                l += l1
                        l_1 += 1
                        
                elif Format_choose == "ODI":
                     while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                elif Format_choose == "TEST":
                    while True and a+b+c+e+f+g+h+j+k+l < Total_score +1:
                         l1 = random.randint(0,6)
                         L1 = random.randint(0,4)
                         if l1 == 0 and L1 == 0:
                             l_1 += 1
                             wick += 1
                             break
                         l = l + l1
                         l_1 += 1
                print(l,end="\t")
        
                print((l_1))

                print("--------------------------------")
              

                Total_score1 = a+b+c+e+f+g+h+j+k+l 

                Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                abc = Total_balls1%6
                print("Total Score :",Total_score1,"/",wick,end="\n")
                print("Total overs :",(Total_balls1//6+(abc/10)))


                print("--------------------------------")


                if Format_choose == "TEST":
                    if Total_score>Total_score1:
                        print(y,"WON the match by",(Total_score - Total_score1),"runs")
                    elif Total_score<Total_score1:
                        print(x,"WON the match by",(Total_score1 - Total_score),"runs")
                    elif Total_score == Total_score1:
                        print("Match is DRAWN")
                else:
                    if Total_score > Total_score1:
                        print(y,"WON the match by",(Total_score - Total_score1),"runs")
                    elif Total_score < Total_score1:
                        print(x,"WON the match by",(10-wick))
                
        

        elif y == "ENG":
                    wick = 0
                    print("Jason Roy",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("J Bairstow",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120:
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Dawid Malan",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Jos Butler",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120:
                            e1 = random.randint(0,6)
                            
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Eoin Morgan",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120:
                            f1 = random.randint(0,7)
                        
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Ben stokes",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120:
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Chris Wokes",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                            
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Moeen Ali",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120:
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jofra Archer",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120:
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)

                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Mark Wood",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120:
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True:
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")
                  

                    Total_score = a+b+c+e+f+g+h+j+k+l 

                    Total_balls = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc2 = Total_balls%6 
                    print("Total Score :",Total_score,"/",wick,end="\n")
                    print("Total overs :",(Total_balls//6+(abc2/10)))


                    print("--------------------------------")
                

                    print(x)


                    print("--------------------------------")

                    print("Player name" ,end="\t")
                    print("Score" ,end="\t")
                    print("No of balls played")

                    wick = 0
                    print("Rohit Sharma",end="\t")
                    a = 0
                    a_1 = 0
                    if Format_choose == "T20":
                        while a_1 < 120 and a < Total_score +1:
                            a1 = random.randint(0,6)
                            A1 = random.randint(0,1)
                            if a1 == 5 and A1 == 0:
                                a_1 += 1
                                wick += 1
                                break
                            if a1 != 5:
                                if a1 == 3:
                                    a = a + 2
                                else:
                                    a = a + a1
                            a_1 += 1
                    elif Format_choose =="ODI":
                         while a_1 < 300 and a < Total_score +1 :
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    elif Format_choose == "TEST":
                        while True and a < Total_score +1:
                             a1 = random.randint(0,6)
                             A1 = random.randint(0,4)
                             if a1 == 0 and A1 == 0:
                                 a_1 += 1
                                 wick += 1
                                 break
                             a = a + a1
                             a_1 += 1
                    print(a,end="\t")
            
                    print((a_1))

                        


                    print("KL Rahul",end="\t")
                    b = 0
                    b_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 ) < 120 and a+b < Total_score+1 :
                            b1 = random.randint(0,6)
                            
                            B1 = random.randint(0,1)
                            if b1 == 5 and B1 == 0:
                                b_1 += 1
                                wick += 1
                                break
                            if b1 != 5:
                                if b1 == 3:
                                    b = b + 2
                                else:
                                    b = b + b1
                            b_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 ) < 300 and a+b < Total_score+1 :
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b < Total_score +1:
                             b1 = random.randint(0,6)
                             B1 = random.randint(0,4)
                             if b1 == 0 and B1 == 0:
                                 b_1 += 1
                                 wick += 1
                                 break
                             b = b + b1
                             b_1 += 1
                    print(b,end="\t")
            
                    print((b_1))


                    print("Virat Kholi",end="\t")
                    c = 0
                    c_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 ) < 120 and a+b+c < Total_score +1:
                            c1 = random.randint(0,6)
                            
                            C1 = random.randint(0,1)
                            if c1 == 5 and C1 == 0:
                                c_1 += 1
                                wick += 1
                                break
                            if c1 != 5:
                                if c1 == 3:
                                    c += 2
                                else:
                                    c += c1
                            c_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 ) < 300 and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c < Total_score +1:
                             c1 = random.randint(0,6)
                             C1 = random.randint(0,4)
                             if c1 == 0 and C1 == 0:
                                 c_1 += 1
                                 wick += 1
                                 break
                             c = c + c1
                             c_1 += 1
                    print(c,end="\t")
            
                    print((c_1))


                    print("Shreyas Iyer",end="\t")
                    e = 0
                    e_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 ) < 120 and a+b+c+e < Total_score+1 :
                            e1 = random.randint(0,6)
                           
                            E1 = random.randint(0,1)
                            if e1 == 5 and E1 == 0:
                                e_1 += 1
                                wick += 1
                                break
                            if e1 != 5: 
                                if e1 == 3:
                                    e += 1
                                else:
                                    e += e1
                            e_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 ) < 300 and a+b+c+e < Total_score+1 :
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e < Total_score +1:
                             e1 = random.randint(0,6)
                             E1 = random.randint(0,4)
                             if e1 == 0 and E1 == 0:
                                 e_1 += 1
                                 wick += 1
                                 break
                             e += e1
                             e_1 += 1
                    print(e,end="\t")
            
                    print((e_1))


                    print("Rishabh Pant",end="\t")
                    f = 0
                    f_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 120 and a+b+c+e+f < Total_score +1:
                            f1 = random.randint(0,7)
                         
                            F1 = random.randint(0,1)
                            if f1 == 5 and F1 == 0:
                                f_1 += 1
                                wick += 1
                                break
                            if f1 != 5:
                                if f1 == 3:
                                    f += 2
                                else:
                                    f += f1
                            f_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 ) < 300 and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f < Total_score+1 :
                             f1 = random.randint(0,6)
                             F1 = random.randint(0,4)
                             if f1 == 0 and F1 == 0:
                                 f_1 += 1
                                 wick += 1
                                 break
                             f += f1
                             f_1 += 1
                    print(f,end="\t")
            
                    print((f_1))

                    print("Hardik Pandya",end="\t")
                    g = 0
                    g_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 120 and a+b+c+e+f+g < Total_score+1 :
                            g1 = random.randint(0,6)
                            G1 = random.randint(0,1)
                            
                            if g1 == 5 and G1 ==0:
                                g_1 += 1
                                wick += 1
                                break
                            if g1 != 5:
                                if g1 == 3:
                                    g += 1
                                else:
                                    g += g1
                            g_1 += 1
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1) < 300 and a+b+c+e+f+g < Total_score+1 :
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g < Total_score +1:
                             g1 = random.randint(0,6)
                             G1 = random.randint(0,4)
                             if g1 == 0 and G1 == 0:
                                 g_1 += 1
                                 wick += 1
                                 break
                             g = g + g1
                             g_1 += 1
                    print(g,end="\t")
            
                    print((g_1))


                    print("Navdeep Saini",end="\t")
                    h = 0
                    h_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 ) < 120 and a+b+c+e+f+g+h < Total_score +1:
                            h1 = random.randint(0,6)
                            H1 = random.randint(0,1)
                           
                            if h1 == 5 and H1 == 0:
                                h_1 += 1
                                wick += 1
                                break
                            if h1 != 5:
                                if h1 == 3:
                                    h += 1
                                elif h1 == 2:
                                    h += 1
                                else:
                                    h += h1
                            h_1 += 1
                            
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1) < 300 and a+b+c+e+f+g+h < Total_score +1:
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h < Total_score+1 :
                             h1 = random.randint(0,6)
                             H1 = random.randint(0,4)
                             if h1 == 0 and H1 == 0:
                                 h_1 += 1
                                 wick += 1
                                 break
                             h += h1
                             h_1 += 1
                    print(h,end="\t")
            
                    print((h_1))



                    print("Mohd Shami",end="\t")
                    j = 0
                    j_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 ) < 120 and a+b+c+e+f+g+h+j < Total_score+1 :
                            j1 = random.randint(0,6)
                            J1 = random.randint(0,1)
                            
                            if j1 == 5 and J1 == 0:
                                j_1 += 1
                                wick += 1
                                break
                            if j1 != 5:
                                if j1 == 3:
                                    j += 0
                                elif j1 == 2:
                                    j += 1
                                else:
                                    j += j1
                            j_1 += 1
                        
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1) < 300 and a+b+c+e+f+g+h+j < Total_score+1:
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j < Total_score+1 :
                             j1 = random.randint(0,6)
                             J1 = random.randint(0,4)
                             if j1 == 0 and J1 == 0:
                                 j_1 += 1
                                 wick += 1
                                 break
                             j += j1
                             j_1 += 1
                    print(j,end="\t")
            
                    print((j_1))



                    print("Jaspreet Bumrah",end="\t")
                    k = 0
                    k_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 ) < 120 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                            k1 = random.randint(0,7)
                            K1 = random.randint(0,1)
                            
                            if k1 == 5 and K1 == 0:
                                k_1 += 1
                                wick += 1
                                break
                            if k1 != 5:
                                if k1 == 3:
                                    k += 0
                                elif k1 == 2:
                                    k += 0
                                elif k1 == 6:
                                    k += 4
                                else:
                                    k += k1
                            k_1 += 1
                           
                    elif Format_choose =="ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1) < 300 and a+b+c+e+f+g+h+j+k < Total_score+1 :
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k < Total_score +1:
                             k1 = random.randint(0,6)
                             K1 = random.randint(0,4)
                             if k1 == 0 and K1 == 0:
                                 k_1 += 1
                                 wick += 1
                                 break
                             k += k1
                             k_1 += 1
                    print(k,end="\t")
            
                    print((k_1))



                    print("Yuzi Chahal",end="\t")
                    l = 0
                    l_1 = 0
                    if Format_choose == "T20":
                        while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 120 and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                            l1 = random.randint(0,5)
                            L1 = random.randint(0,1)
                            if l1 == 5 and L1 == 0:
                                l_1 += 1
                                wick += 1
                                break
                            if l1 != 5:
                                if l1 == 3:
                                    l += 0
                                elif l1 == 2:
                                    l += 0
                                elif l1 == 6:
                                    l += 2
                                else:
                                    l += l1
                            l_1 += 1
                            
                    elif Format_choose == "ODI":
                         while (a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1) < 300 and a+b+c+e+f+g+h+j+k+l < Total_score +1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    elif Format_choose == "TEST":
                        while True and a+b+c+e+f+g+h+j+k+l < Total_score+1 :
                             l1 = random.randint(0,6)
                             L1 = random.randint(0,4)
                             if l1 == 0 and L1 == 0:
                                 l_1 += 1
                                 wick += 1
                                 break
                             l = l + l1
                             l_1 += 1
                    print(l,end="\t")
            
                    print((l_1))

                    print("--------------------------------")

                    Total_score1 = a+b+c+e+f+g+h+j+k+l 

                    Total_balls1 = a_1 + b_1 + c_1 + e_1 + f_1 + g_1 + h_1 + j_1 + k_1 + l_1
                    abc3 = Total_balls%6
                    print("Total Score :",Total_score1,"/",wick,end="\n")
                    print("Total overs :",(Total_balls1//6+(abc3/10)))


                    print("--------------------------------")


                    if Format_choose == "TEST":
                        if Total_score > Total_score1:
                            print(y,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score<Total_score1:
                            print(x,"WON the match by",(Total_score1 - Total_score),"runs")
                        elif Total_score == Total_score1:
                            print("Match is DRAWN")
                    else:
                        if Total_score > Total_score1:
                            print(y,"WON the match by",(Total_score - Total_score1),"runs")
                        elif Total_score < Total_score1:
                            print(x,"WON the match by",(10-wick),"WICKETS")



            

        



























