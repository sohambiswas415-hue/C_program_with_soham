# C_program_with_soham

/*Write a program to accept marks of five subjects and calculate the total marks and
percentage.*/
#include <stdio.h>
int main()
{
    int marks, i, n, avg, total = 0;
    float percen;
    printf("Enter the number of subjects: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
    {
        printf("Enter marks in subject: ");
        scanf("%d", &marks);
        total += marks; 
    }
    
    printf("Total marks of %d subjects is:%d\n ", n, total);
    avg = total / n;
    printf("Average makrks of %d subjects is: %d\n", n, avg);
    percen = (total / 80) * 100; 
    printf("Percentage makrks of %d subjects is: %.2f\n", n, percen);

    switch (avg / 10)
    {
    case 4:
        printf("Grade D\n");
        break;
    case 5:
        printf("Grade C\n");
        break;
    case 6:
        printf("Grade B\n");
        break;
    case 7:
        printf("Grade A\n");
        break;
    case 8:
        printf("Grade E\n");
        break;
    case 9:
        printf("Grade O\n");
        break;
    case 10:
        printf("Grade O\n");
        break;
    default:
        printf("Fail, Better luck next time!");
            
            
    }
    return 0;
}
