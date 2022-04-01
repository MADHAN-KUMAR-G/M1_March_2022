#include<stdio.h>

#define CANDIDATE_COUNT

#define CANDIDATE1 "Shri M.K. Stalin"
#define CANDIDATE2 "Shri YS Jagan Mohan Reddy"
#define CANDIDATE3 "Shri Pema Khandu"
#define CANDIDATE4 "Shri Nitish Kumar"
#define CANDIDATE5 "Shri Bhupesh Baghel"
#define CANDIDATE6 "Shri Pushkar Singh Dhami"
#define CANDIDATE7 "Shri N. Rangaswamy"
#define CANDIDATE8 "Shri Ashok Gehlot"
#define CANDIDATE9 "Shri PS Golay"
#define CANDIDATE10 "Shri Jairam Thakur"

int votesCount1=0, votesCount2=0, votesCount3=0, votesCount4=0,votesCount5=0,votesCount6=0,votesCount7=0,votesCount8=0,votesCount9=0,votesCount10=0,spoiledtvotes=0;

void castVote(){
int choice;    
printf("\n\n ### Please choose your Candidate ####\n\n");
printf("\n 1. %s", CANDIDATE1);
printf("\n 2. %s", CANDIDATE2);
printf("\n 3. %s", CANDIDATE3);
printf("\n 4. %s", CANDIDATE4);
printf("\n 5. %s", CANDIDATE5);
printf("\n 6. %s", CANDIDATE6);
printf("\n 7. %s", CANDIDATE7);
printf("\n 8. %s", CANDIDATE8);
printf("\n 9. %s", CANDIDATE9);
printf("\n 10. %s", CANDIDATE10);
printf("\n 11. %s", "None of These");
printf("\n\n Input your choice (1 - 10) : ");
scanf("%d",&choice);
switch(choice){
    case 1:
	{
	
	  votesCount1++;
	break;
}
    case 2: 
	{
	votesCount2++; 
	break;
}
    case 3:
	{
	  
	votesCount3++;
	break;
}
    case 4: 
		{
		
	votesCount4++;
	break;
}
    case 5:
	{
	  votesCount5++; 
	break;
}
    case 6:
    	{
		
	 votesCount6++; 
	break;
}
    case 7: 
	{
	votesCount7++; 
	break;
}
    case 8: 
    {
	
	votesCount8++; 
	break;
}
    case 9:
	{
	  
	votesCount9++; 
	break;
}
    case 10:
	{
	  votesCount10++; 
	break;
}
    case 11: spoiledtvotes++; 
	break;
    default: printf("\n Error: Wrong Choice !! Please retry");
             //hold the screen
             getchar();
}
printf("\n thanks for vote !!");
}
void votesCount(){
printf("\n\n ##### Voting Statics ####");
printf("\n %s - %d ", CANDIDATE1, votesCount1);
printf("\n %s - %d ", CANDIDATE2, votesCount2);
printf("\n %s - %d ", CANDIDATE3, votesCount3);
printf("\n %s - %d ", CANDIDATE4, votesCount4);
printf("\n %s - %d ", CANDIDATE5, votesCount5);
printf("\n %s - %d ", CANDIDATE6, votesCount6);
printf("\n %s - %d ", CANDIDATE7, votesCount7);
printf("\n %s - %d ", CANDIDATE8, votesCount8);
printf("\n %s - %d ", CANDIDATE9, votesCount9);
printf("\n %s - %d ", CANDIDATE10, votesCount10);
printf("\n %s - %d ", "Spoiled Votes", spoiledtvotes); 
}
void getLeadingCandidate(){
    printf("\n\n  #### Leading Candiate ####\n\n");
    if(votesCount1 > votesCount2 && votesCount1 > votesCount3 && votesCount1 >votesCount4 && votesCount1 >votesCount5 && votesCount1 >votesCount6 && votesCount1 >votesCount7 && votesCount1 >votesCount8 && votesCount1 >votesCount9 && votesCount1 >votesCount10 )
    printf("[%s]",CANDIDATE1);
    else if (votesCount2>votesCount3 && votesCount2>votesCount4 && votesCount2 >votesCount1 && votesCount2>votesCount5 && votesCount2>votesCount6 && votesCount2>votesCount7 && votesCount2>votesCount8 && votesCount2>votesCount9 && votesCount2>votesCount10)
    printf("[%s]",CANDIDATE2);
    else if(votesCount3>votesCount4 && votesCount3>votesCount2 && votesCount3 >votesCount1 && votesCount3 >votesCount5 && votesCount3 >votesCount6 && votesCount3 >votesCount7 && votesCount3 >votesCount8 && votesCount3 >votesCount9 && votesCount3 >votesCount10)
    printf("[%s]",CANDIDATE3);
    else if(votesCount4>votesCount1 && votesCount4>votesCount2 && votesCount4 >votesCount3 && votesCount4 >votesCount5 && votesCount4 >votesCount6 && votesCount4 >votesCount7 && votesCount4 >votesCount8 && votesCount4 >votesCount9 && votesCount4 >votesCount10)
    printf("[%s]",CANDIDATE4);
    else if(votesCount5>votesCount1 && votesCount5>votesCount2 && votesCount5>votesCount3 && votesCount5>votesCount4 && votesCount5>votesCount6 && votesCount5>votesCount7 && votesCount5>votesCount8 && votesCount5>votesCount9 && votesCount5>votesCount10 )
    printf("[%s]",CANDIDATE5);
    else if(votesCount6>votesCount1 && votesCount6>votesCount2 && votesCount6>votesCount3 && votesCount6>votesCount4 && votesCount6>votesCount5 && votesCount6>votesCount7 && votesCount6>votesCount8 && votesCount6>votesCount9 && votesCount6>votesCount10 )
    printf("[%s]",CANDIDATE6);
    else if(votesCount6>votesCount1 && votesCount6>votesCount2 && votesCount6>votesCount3 && votesCount6>votesCount4 && votesCount6>votesCount5 && votesCount6>votesCount7 && votesCount6>votesCount8 && votesCount6>votesCount9 && votesCount6>votesCount10 )
    printf("[%s]",CANDIDATE7);
    else if(votesCount8>votesCount1 && votesCount8>votesCount2 && votesCount8>votesCount3 && votesCount8>votesCount4 && votesCount8>votesCount5 && votesCount8>votesCount6 && votesCount8>votesCount7 && votesCount8>votesCount9 && votesCount8>votesCount10 )
    printf("[%s]",CANDIDATE8);
    else if(votesCount9>votesCount1 && votesCount9>votesCount2 && votesCount9>votesCount3 && votesCount9>votesCount4 && votesCount9>votesCount6 && votesCount9>votesCount7 && votesCount9>votesCount8 && votesCount9>votesCount5 && votesCount9>votesCount10 )
    printf("[%s]",CANDIDATE9);
    else if(votesCount10>votesCount1 && votesCount10>votesCount2 && votesCount10>votesCount3 && votesCount10>votesCount4 && votesCount10>votesCount5 && votesCount10>votesCount6 && votesCount10>votesCount7 && votesCount10>votesCount10 && votesCount10>votesCount9 )
    printf("[%s]",CANDIDATE10);
    else
    printf("----- Warning !!! No-win situation----");       
}
int main()
{
int i;
int choice;
do{
printf("\n\n ###### Welcome to Election/Voting 2022 #####");
printf("\n\n 1. Cast the Vote");
printf("\n 2. Find Vote Count");
printf("\n 3. Find leading Candidate");
printf("\n 0. Exit");
printf("\n\n Please enter your choice : ");
scanf("%d", &choice);
switch(choice)
{
case 1: castVote();
break;
case 2: votesCount();
break;
case 3: getLeadingCandidate();
break;
default: printf("\n Error: Invalid Choice");
}
}while(choice!=0);
getchar();
return 0;
}
