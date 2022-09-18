from os import stat
from pstats import Stats
from secrets import choice
from sre_parse import State


def ostan(dic):
    stats, center = input("Enter a number:").split()
    dic[State] = center
def shahr (dic):
    stats = input(" Enter a number :") 
    if state in dic:
        print("State","Center")
        print(state,dic[state])
    else:
        print("State",state,"not found")
        input("prees ok to contineu:")
def display(dic):
    print("State","center")
    print("-"*20)
    for state in dic:
        print(state,dic[state])
def update (dic):
    state, center = input("Enter a number:").split()
    d = {state:center}
    dic.update(d)
def delet (dic):
    state = input("Enter a number:")
    if state in dic:
        del dic[state]
        print("state",state,"deleted")
    else:
        print("state",state,"not found")
    input("prees ok to continue:")
def menu ():
    print("1.Enter data to dictionary")
    print("2.search a state")
    print("3.delet a state")
    print("4.update the state center of dictonary")
    print("5.display the contents of dictionary")
    print("6.Exit")
    choice = int(input("Enter your select (1-6):"))        
    return choice
stdic = dict()
while True:
    c=menu()
    if c==1:
        dicostan(stdic)
    elif c==2:
        dicshar(stdic)
    elif c==3:
        dicdelet(stdic)
    elif c==4:
        dicupdate(stdic)
    elif c==5:
        dicdisplay(stdic)
    else:
        break                        
