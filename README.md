# Student-Records
This is the program regarding Student Records.

#sourcecode
#include <stdio.h>
#include <stdlib.h>
struct student 
{
    char first_name[50], last_name[50], sec[10];
    int roll;
    float marks;
	
} a[5];

int main()
{
	//a-z = 97-122
	//A-Z = 65-90
	
    int i;
    printf("Enter information of students:\n");

    // Input
    for (i=0 ; i < 3; ++i) 
	{
        a[i].roll = i + 1;
        printf("\nFor roll number: %d ,\n", a[i].roll);
		
        printf("Enter first name: ");
        scanf("%s", a[i].first_name);
		
        printf("Enter last name: ");
        scanf("%s", a[i].last_name);
		
		printf("Enter your Section: ");
        scanf("%s", a[i].sec);
		
        printf("Enter Total Marks: ");
        scanf("%f", &a[i].marks);
		
		printf("\n");
    }
		printf("\n");
		
Output
	
    for (i = 0; i < 3; ++i)
	{
        printf("\nRoll number: %d\n", i + 1);
		
        printf("First name: ");
        puts(a[i].first_name);
		
        printf("Last name: ");
        puts(a[i].last_name);
		
		printf("Section: ");
        puts(a[i].sec);
		
        printf("Marks scored: %.2f", a[i].marks);
        printf("\n");
    }
    return 0;
}
