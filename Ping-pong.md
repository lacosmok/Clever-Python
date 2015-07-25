# Clever-Python
Clever python codes that i need to know

In python u can set values as quick functions and then just return it:
def service(score):
  turn = sum(int(i) for i in score.split(":"))
  condition = (turn%10 < 5) if turn < 40 else (turn%4 < 2)
  return "first" if condition else "second"

Code to compare:
def service(score):
    score=score.split(":") 
    print score[0], score[1]  
    if (int(score[1]))<=20 and int(score[0])<=20:
        score=int(score[0])+int(score[1])
        x=score/5
        print x
        if x%2==1:
            return "second"
        else:
            return "first"
    else:
    	score=int(score[0])+int(score[1])-40
        score=score/2
        print score
        if score%2==0: 
        	return "first"
        else:
        	return "second"
  
