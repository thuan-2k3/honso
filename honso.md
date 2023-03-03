#include<stdio.h>
#include<conio.h>
struct honso
{
    int tuso, mauso, songuyen ;
};

typedef struct honso HS ;
void nhaptuso (HS );
void nhapmauso ( HS );
void nhapsonguyen( HS );
void xuathonso ( HS );

void nhaptuso (HS hs)
{
    printf("nhap vao tu so:");
    scanf("%d", &hs.tuso );
    
};

void nhapmauso (HS hs)
{do {
    printf("nhap vao mau so:");
    scanf("%d", &hs.mauso );
    
    if( hs.mauso == 0)
        printf("vui long nhap lai ");
}
    while ( hs.mauso == 0) ;

};

void nhapsonguyen (HS hs)
{
    printf("nhap vao so nguyen : ");
    scanf("%d", &hs.songuyen );

}

void xuathonso (HS hs ) 
{
    printf("%d \b %d/%d", hs.songuyen, hs.tuso, hs.mauso );
}

int main ()
{
    HS hs ;
    nhaptuso (hs);
    nhapmauso (hs) ;
    nhapsonguyen (hs) ;
   xuathonso (hs) ;
    return 0;

}









