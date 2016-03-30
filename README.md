# pset2

#include <stdio.h>
#include <cs50.h>
#include <string.h>
#include <stdlib.h>
#include <ctype.h>



int key;
int newnumber; 

int main(int argc, string argv[])

{
   
    //get the key  - user enters ./caesar 2
    int key = atoi(argv[1]); // declaring the key variable & converting string "key" to an integer that can be validated
    
        if (key <= 0)   // if key is less than or equal to zero, return a 0 [false]; restart program 
        {
            return 0;
            printf("You need to input an integer greater than 0. Try again.\n");  //tell the user why they need to try again
        }
    
        //get the plaintext message from the user 
        else 
        {
            printf("Please type a short message to encipher:\n");
        }
        
        string message = GetString();
    
        return 0;
}

    if (argc == 2)
    {
        return 0;
    }
    
    else if (argc < 2)
    {
        printf("Please input one integer greater than zero:")
        return 1;
    }
    
    else if (argc > 2)
    {
        printf("Please input *only* one cipher (integer):")
        return 1;
    }
    
        //dealing with the wrap-around
            if (key >= 26)
            {
                key = (key % 26);
            }
        
        
    // encipher the message
    for(int i = 0, length = strlen(message); i < length; i++)
        {
            newnumber[i] = message[i] + key;
            
            if(isupper(message[i] && (newnumber > 'Z'))
            {
                newnumber = newnumber - 26;
            }
            
            if(islower(message[i] && (newnumber > 'z'))
            {
                newnumber = newnumber - 26;
            }
            
            if(isalspha(message[i]))
            {
                printf("%c", newnumber);
            }
            
            else
            {
                printf(" ", newnumber);
            }
        }
         
         printf("" "\n");
         return 0;
  }  
        
       

