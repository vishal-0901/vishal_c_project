#include <stdio.h>


void main()
{
    FILE *fp;
    char name[300];

    //clrscr();

    // 1. Writing data into file
    fp = fopen("ruby.txt", "w");

    if (fp == NULL)
    {
        printf("File cannot be opened");
    
        return;
    }

    fprintf(fp, "Before you joined our class, different teachers taught us C programmingInitially, I found it a little difficult to understand, but gradually, I started understanding the concepts better. Thank you, Sir, for coming to our class and helping us improve our programming knowledge.  ");

    fclose(fp);

    printf("ruby written successfully\n");


    // 2. Appending data into file
    fp = fopen("student.txt", "a");

    if (fp == NULL)
    {
        printf("File cannot be opened");
        
        return;
    }

    fprintf(fp, "\nAfter you started teaching us, I began to understand the concepts better, and I was able to perform well in my exams. Your teaching has helped me gain more confidence in C programming. Thank you, Sir, for coming to our class and helping us improve our knowledge and skills ");

    fclose(fp);

    printf("Data appended successfully\n");


    // 3. Reading data from file
    fp = fopen("student.txt", "r");

    if (fp == NULL)
    {
        printf("File cannot be opened");
        
        return;
    }

    printf("\nFile Contents:\n");

    while (fgets(name, sizeof(name), fp) != NULL)
    {
        printf("%s", name);
    }

    fclose(fp);


}
