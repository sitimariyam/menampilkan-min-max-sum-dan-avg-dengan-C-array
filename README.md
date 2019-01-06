#   MENAMPILKAN MIN, MAX, SUM, DAN AVG C++ ARRAY

         #include<iostream>
           #include<conio.h>
           #include<stdlib.h>
           using namespace std;
           int main()
           {
           float n,min,max,bil,i,jum,rata2;
           int pilih;


           cout<<"MENGHITUNG NILAI JUMLAH, RATA-RATA, MAKSIMAL & MINIMAL "<<endl;

          out<<"Masukkan jumlah bilangan : "; cin>>n;
     jum=0;
     min=100;
     max=0;
     for(i=1;i<=n;i++){
     cout<<"Masukan N ke-"<<i<<" : "; cin>>bil;
     jum=jum+bil;
     if (max<bil){
       max=bil;
     } else if(min>bil){
       min=bil;
     }
     rata2=jum/n;
     }
    cout<<endl;

    menu:
    cout<<endl;
    cout<<"Pilihan : "<<endl;
    cout<<"1. Nilai Jumlah "<<endl;
    cout<<"2. Nilai Rata-rata "<<endl;
    cout<<"3. Nilai Max "<<endl;
    cout<<"4. Nilai Min "<<endl;
    cout<<"Pilih hasil mana yang ingin anda ketahui : ";
    cin>>pilih;

    switch(pilih){
    case 1:

    cout<<"Nilai Jumlah : "<<jum<<endl;
    getch();
    goto menu;

    case 2:
    cout<<"Nilai Rata-rata : "<<rata2<<endl<<endl;
    getch();
    goto menu;

    case 3:
    cout<<"Nilai Maximum : "<<max;
    getch();
    goto menu;
    case 4:
    cout<<"Nilai Minimum : "<<min;
      getch();
     goto menu;
    }



    return 0;

    }
