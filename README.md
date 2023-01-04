# chatbot
# AI project

#include<stdio.h>                                 
#include<conio.h>
#include<string.h>
#include<time.h>
#include<stdlib.h>

char user_input[];
int main()
{   system("cls");
    printf("welcome to AI chat bot\n");
    while(1)
    {
     printf("user ==> ");
     gets(user_input);
     if(strcmp(user_input,"exit")==0)
     {
         system("cls");
         printf("bot ==> ok byy\n");
         break;
     }
     else if(strcmp(user_input,"hi")==0)
     {
         printf("bot ==> hi sir\n");
     }
     else if(strcmp(user_input,"open chrome")==0)
     {
         printf("ok sir , opening chrome browser \n");
         system("start chrome");
     }
     else if(strcmp(user_input,"open notepad")==0)
     {
         printf("ok sir , opening notpad editor \n");
         system("start notepad");
     }
     else if(strcmp(user_input,"open cmd")==0)
     {
         printf("ok sir , opening cmd terminal \n");
         system("start cmd");
     }
     else if(strcmp(user_input,"time")==0)
     {
         time_t s, val =1 ;
         struct tm* current_time;
         //time in second
         s = time(NULL);
         current_time = localtime(&s);
         //print time in minute
         //print hour and second
         printf("bot ==> %02d:%02d:%02d\n",current_time->tm_hour,current_time->tm_min,current_time->tm_sec);
     }
     else if(strcmp(user_input,"open youtube")==0)
     {
        printf("ok sir , opening youtube \n");   
        system("start http://youtube.com");   
     }
    }
    // Returning 
    return 0;
}
