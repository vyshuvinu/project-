#include <stdio.h>
#include <string.h>

//Compiler version gcc  6.3.0

int main()
{
  char name[40], empname[40];
  int age, choice;
  float basicsalary;
  
  printf("1.Add records \n");
 
  printf("2.Modify records\n");
  printf("3.Delete records\n");
  printf("4.Exit\n");
  printf("your choice:");
  scanf("\n%d", &choice);
  switch (choice)
    {
      case 1:
        
          
        printf("\n enter the name:");
          scanf("%s", &name);
          printf("enter the age\n");
          scanf("%d", &age);
          printf("enter the basic salary: \n");
          scanf("%f", &basicsalary);
          printf("add another record\n");
          break;
          
            case 2:
                 printf("\n enter the name:");
          scanf("%s", &name);
              printf("enter the name to modify:\n");
              scanf("%s", &empname);
           
              if(strcmp(name, empname)==0)
              printf("enter the name, age, basicsalary\n");
              scanf("%s%d%f", &name, &age, &basicsalary);
              break;
              case 3:
                printf("\n enter the name:");
          scanf("%s", &name);
                printf("enter the name of employee to delete :");
                scanf("%s", &empname);
                if(strcmp(name, empname)!=0)
                printf("delete record");
                break;
                case 4:
                  printf("exit\n");break;
        
    }
    
  
  
  return 0;
}

