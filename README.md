# Quiz-game
#include<iostream>
using namespace std;
int main()
{
int finalResult=0;
char playAgain;
int playQuiz(void);
play:
finalResult=playQuiz();
cout<<"your score is"<<finalResult<<endl;
if(finalResult>=6)
{
cout<<"you are pass"<<endl;
cout<<"Do you want to play QUIZ again y or n?"<<endl;
cin>>playAgain;
if(playAgain=='y'||playAgain=='Y')
{
 goto play;
}
else
{
 cout<<"thanku you to play Quiz!"<<endl;
}
}
else
{
cout<<"you are fail"<<endl;
cout<<"Do you want to play QUIZ again y or n?"<<endl;
cin>>playAgain;
if(playAgain=='y'||playAgain=='Y')
{
 playQuiz();
}
else
{
 cout<<"thanku you to play Quiz!"<<endl;
}
}
}
int playquiz()
{
char c;
char option;
int score=0;
playInsideFunction:
cout<<"--------welcome to quize Game--------"<<endl;
cout<<"------please follow instructions-----"<<endl;
cout<<"step 1:quiz contains total 10 questions"<<endl;
cout<<"step 2:you will given 1 marks for each right ans"<<endl;
cout<<"step 3: there will be no negataive marking"<<endl;
cout<<"step 4:please press s to start the quiz"<<endl;
cout<<"step 5:please select option a,b,c,d"<<endl;
cout<<"step 6:If you score >=6,you will pass the quiz"<<endl;
cin>>c;
if(c=='s'||c=='s')
{
cout<<"Q1. what is the capital of india"<<endl;
cout<<"(a)Delhi(b)Mumbai(c)Kolkata(d)Chennai"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q2. who is the prime minister of india"<<endl;
cout<<"(a)Narendra Modi(b)Aditynath(c)Kejriwal(d)Nitin"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q3. what is the national bird of India"<<endl;
cout<<"(a)Peacock(b)Sparrow(c)Pigeon(d)Parrot"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q4. what is the national animal of India"<<endl;
cout<<"(a)Tiger(b)Lion(c)Zebra(d)Leopard"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q5. what is the national flower of India"<<endl;
cout<<"(a)Lotus(b)Rose(c)Lily(d)sunflower"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q6.who is the chief minister of up"<<endl;
cout<<"(a)Aditynath(b)Kejriwal(c)Nitin(d)Raghunath"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q7. what is the capital of up"<<endl;
cout<<"(a)Lukhnow(b)Praygraj(c)Mirzapur(d)Itwawa"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q8. what is the capital of jharkhand"<<endl;
cout<<"(a)Ranchi(b)Ramgarh(c)Plamu(d)Dhanbad"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q9. who is the leader of congress"<<endl;
cout<<"(a)Rahul(b)Sonia(c)Roshan(d)Rohit"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
cout<<"Q10. which one of the following state comes in North"<<endl;
cout<<"(a)Delhi(b)Banglore(c)chennai(d)Kerla"<<endl;
cin>>option;
if(option=='a'||option=='A')
{
score=score+1;
}
else
{
score=score+0;
}
}
else
{
cout<<"you have enterd  wrong value,please enter s"<<endl;
goto playInsideFunction;
}
return score;


}
