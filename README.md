# 2021homework
#include<stdio.h>
int main(int argc, char**argv)
{
    printf("現在的 argc是:%d\n",argc);
    for(int i=0; i<argc; i++)
    {
        printf("argv[%d]是:%s\n",i,argv[i]);
    }
}
