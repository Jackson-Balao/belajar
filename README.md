# belajar
matrikspenjumlahan
saya ingin menjadi iron man



website,matriks,penjumlahan
link,belajar,matriks





#include <iostream>

using namespace std;
, int kolom);

int main()
{
    cout << "Matriks input" << endl;
    int baris = 4;
    int kolom = 5;

    int mata[10][10];
    int matb[10][10];
    int matH[10][10];

    inputDataMat(mata, baris, kolom);
    inputDataMat(matb, baris, kolom);

    cout << "Tampilkan data matriks 1: " << endl;
    tampilDataMat(mata, baris,kolom);

    cout << endl << "Tampilkan data matriks 2: " << endl;
    tampilDataMat(matb, baris, kolom);

    cout << endl << endl << "Hasil penjumalahan matriks 1 dan 2: " << endl;
    jumlahkanMatriks(mata, matb, matH, baris, kolom);
    tampilDataMat(matH, baris, kolom);

    cout << endl << endl << "Hasil perkalian matriks 1 dan 2: " << endl;
    kalikanMatriks(mata, matb, matH, baris, kolom);
    tampilDataMat(matH, baris, kolom);
    return 0;
}

saya
void inputDataMat (int matA[][10], int baris, int kolom)
{
    // masukkan data
    for (int i=0; i < baris; i++)
    {
        for (int j=0; j < kolom; j++)
        {
            // simpan data
            matA[i][j] = i * j *2;
        }
    }
}

void inputDataMat (int matA[][10], int baris, int kolom);
void tampilDataMat (int matA[][10], int baris, int kolom);
void jumlahkanMatriks (int matA[][10], int matB[][10],
                        int matHasil[][10], int baris, int kolom);
void kalikanMatriks (int matA[][10], int matB[][10],
                        int matHasil[][10], int 
void tampilDataMat (int matA[][10], int baris, int kolom)
{
    for (int i=0; i < baris; i++)
    {
        for (int j=0; j < kolom; j++)
        {
            // tampilkan data
            cout << matA[i][j];
            cout << "\t";
        }
        cout << endl;
    }
}

void jumlahkanMatriks (int matA[][10], int matB[][10],
                    int matHasil[][10], int baris, int kolom)
{
    // penjumlahan matriks
    for (int i=0; i < baris; i++)
    {
        for (int j=0; j < kolom; j++)
        {
            // jumlahkan data
            int jumlah = matA[i][j] + matB[i][j];
            matHasil[i][j] = jumlah;


        }
    }
}


void kalikanMatriks (int matA[][10], int matB[][10],
                    int matHasil[][10], int baris, int kolom)
{
    // perkalian matriks
    for (int i=0; i < baris; i++)
    {
        for (int j=0; j < kolom; j++)
        {
            // kalikan data
            int kali = matA[i][j] * matB[i][j];
            matHasil[i][j] = kali;


        }
    }
}
