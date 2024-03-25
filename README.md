#include <iostream>

using namespace std;

int main()
{
    cout << " Nama : Valentino Silalahi " << endl;
    cout << " Nim  : 2310431015 " << endl;
    cout << " Program Bilangan Fibonacci "<<endl;

    int i,n,f_1,f_2;
    float jumlah,f_n;

    while (true){
    cout <<endl<< " Masukkan Nilai n = ";
    cin >> n;

    f_1 = 1; f_2 = 1;
    jumlah = 2;

    if ( (n >= 3 && n <= 100) || ( n >= 109 && n <= 199 ) )
        { for ( i=3; i <= n; i++ )
            {   f_n = f_1+f_2;
                jumlah += f_n;
                f_2 = f_1;
                f_1 = f_n;
            }
          cout <<endl<< " Bilangan fibonacci ke-"<<n<< " adalah = "<<f_n<<endl;
          cout << " Jumlah bilangan fibonacci dari f_1 sampai f_"<<n<< " adalah = "<<jumlah<<endl;
          break; }
      else { cout <<endl<< " Nilai n yang dimasukkan tidak valid. Silahkan coba lagi. "<<endl; }
    }
}
