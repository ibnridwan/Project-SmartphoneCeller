#include <iostream>
#include <conio.h>
#include <iomanip> //setw()
#include <cstdlib>
using namespace std;

struct Data_node
{
		char alamat[20];
		char nope[20];
       char nama[25];
       char phone[20];
      
       int stts,harga,bayar,kembali;
       
};

struct node
{
      Data_node data;
      node* next;
};
node* arus;
node* depan;
node* belakang;
node* masuk;
node* hapus;

void inisialisasi()
{
      depan = NULL;
      belakang = NULL;
}


void input(Data_node dt)
{
      
      masuk = (node* )malloc(sizeof(node)); //alokasi memori
      masuk->data = dt; //penugasan struktur
      masuk->next = NULL;
      if(depan==NULL)
      {
            depan = masuk;
            belakang = depan;
      }
      else
      {
            belakang->next = masuk;
            belakang = masuk;
      }
}

void hapuss()
{
      node simpan;
      if(depan==NULL)
      {
        cout<<"\t\t\t |=====================================================|"<<endl;
		cout<<"\t\t\t |-----DATA KOSONG , HAPUS TIDAK BISA DILAKUKAKAN------|"<<endl;
		cout<<"\t\t\t |=====================================================|"<<endl;
      }
      else
      {
        simpan.data  = depan ->data;
        cout<<"\t\t\t |=============================================|"<<endl;
		cout<<"\t\t\t |--------------DATA YANG DIHAPUS--------------|"<<endl;
		cout<<"\t\t\t |=============================================|"<<endl;
		cout<<"\t\t\t   NAMA = "<<simpan.data.nama<<endl;;
		cout<<"\t\t\t   Alamat = "<<simpan.data.alamat<<endl;
		cout<<"\t\t\t   No. HP = "<<simpan.data.nope<<endl;
		cout<<"\t\t\t   Pilihan Smartphone = "<<simpan.data.phone<<endl;
		cout<<"\t\t\t   Harga Smartphone =Rp"<<simpan.data.harga<<endl;
		cout<<"\t\t\t   Uang Pembeli =Rp"<<simpan.data.bayar<<endl;
		cout<<"\t\t\t   Sisa Kembalian =Rp"<<simpan.data.kembali<<endl;
		cout<<"\t\t\t |=============================================|"<<endl;

            //hapus depan
            hapus = depan;
            depan = depan->next;
            delete hapus;
      }
}

void cetak()
{
      arus = depan;
      if(depan == NULL)
            cout<<"\ntidak ada data dalam linked list"<<endl;
      else
      {
      	cout<<"\t\t\t |=============================================|"<<endl;
		cout<<"\t\t\t |-------------STRUK DATA PEMBELI--------------|"<<endl;
		cout<<"\t\t\t |=============================================|"<<endl;
            while(arus!=NULL)
            {
            	cout<<"\t\t\t   NAMA = "<<arus->data.nama<<endl;
				cout<<"\t\t\t   Alamat = "<<arus->data.alamat<<endl;
				cout<<"\t\t\t   No. HP = "<<arus->data.nope<<endl;
				cout<<"\t\t\t   Pilihan Smartphone = "<<arus->data.phone<<endl;
				cout<<"\t\t\t   Harga Smartphone =Rp "<<arus->data.harga<<endl;
				cout<<"\t\t\t   Uang Pembeli =Rp "<<arus->data.bayar<<endl;
				cout<<"\t\t\t   Sisa Kembalian =Rp "<<arus->data.kembali<<endl;
		cout<<"\t\t\t |=============================================|"<<endl;
                arus = arus->next;
            }
            cout<<endl;
      }
}

int main()
{
    
    int spek,tipe,beli,satu,dua,merk;
    char pilih,ulang;
    node tmp; 

	do
	{
    system("cls");
    	cout<<"\t\t\t |=========================================|\t\t\t"<<endl;
		cout<<"\t\t\t |------SMARTPHONE CELLER CENTER GOWA------|\t\t\t"<<endl;
		cout<<"\t\t\t |=========================================|\t\t\t"<<endl;
    	cout<<"\t\t\t  Menu : "<<endl;
    	cout<<"\t\t\t   1. Input data"<<endl;
    	cout<<"\t\t\t   2. Hapus data"<<endl;
    	cout<<"\t\t\t   3. Cetak Data"<<endl;
    	cout<<"\t\t\t   4. Exit"<<endl;
    	cout<<"\t\t\t |=========================================|\t\t\t"<<endl;
    	cout<<"\t\t\t  Masukkan pilihan Anda : "; cin>>pilih;
	system("cls");
    switch(pilih)
      {
      case '1' :
            /*
              Pada bagian ini nilai input disimpan pada struct data 
               yang ada pada struct tmp (tmp.data).


              Kemudian tmp.data digunakan sebagai parameter untuk- 

               memanggil fungsi input()
            */
  
    system("cls");
    cout<<"\t\t\t |===============================|\t\t\t"<<endl;
	cout<<"\t\t\t |--Pilih Status Pekerjaan Anda--|"<<endl;
	cout<<"\t\t\t |===============================|\t\t\t"<<endl;
	cout<<"\t\t\t |-----1.Kuliah atau Sekolah-----|\t\t\t"<<endl;
	cout<<"\t\t\t |-----------2.Bekerja-----------|\t\t\t"<<endl;
	cout<<"\t\t\t |--------3.Tidak Bekerja--------|\t\t\t"<<endl;
	cout<<"\t\t\t |===============================|\t\t\t"<<endl;
	cout<<"\t\t\t  Pilihan Anda = "; cin>>tmp.data.stts;
		if (tmp.data.stts==1)
		{
			cout<<"\n\t\t----KAMI MEREKOMENDASIKAN SMARTPHONE SPEK MENENGAH KE BAWAH----\t\t\n"<<endl;
		}
		else if (tmp.data.stts==2)
		{
			cout<<"\n\t\t----KAMI MEREKOMENDASIKAN SMARTPHONE SPEK MENENGAH KE ATAS----\t\t\n"<<endl;
		}
		else if (tmp.data.stts==3)
		{
			cout<<"\n\t\t\t----KAMI MEREKOMENDASIKAN SMARTPHONE SPEK MENENGAH KE BAWAH----\t\tn"<<endl;
		}
	cout<<"\t\t\t |===============================|\t\t\t"<<endl;
	cout<<"\t\t\t |----Masukkan Spesifikasi-------|\t\t\t"<<endl;
	cout<<"\t\t\t |----1. Spek Menengah Keatas----|\t\t\t"<<endl;
	cout<<"\t\t\t |----2. Spek Menengah Kebawah---|\t\t\t"<<endl;
	cout<<"\t\t\t |===============================|\t\t\t"<<endl;
	cout<<"\t\t\t  Pilihan Anda = "; cin>>spek;
	system("cls");
	if (spek==1)
	{
	system("cls");
	cout<<"\t\t\t |============================================|\t\t\t"<<endl;
	cout<<"\t\t\t |--Pilih Merk Smartphone Spesifikasi Tinggi--|\t\t\t"<<endl;
	cout<<"\t\t\t |-----------------1. IPHONE------------------|\t\t\t"<<endl;
	cout<<"\t\t\t |-----------------2. SAMSUNG-----------------|\t\t\t"<<endl;
	cout<<"\t\t\t |============================================|\t\t\t"<<endl;
	cout<<"\t\t\t  Pilihan Anda = "; cin>>merk;
		if (merk==1)
		{
			cout<<"\t\t\t |===========================|\t\t\t"<<endl;
			cout<<"\t\t\t |--Pilih Jenis Tipe Iphone--|\t\t\t"<<endl;
			cout<<"\t\t\t |-------1. IPHONE X---------|\t\t\t"<<endl;
			cout<<"\t\t\t |-------2. IPHONE 9---------|\t\t\t"<<endl;
			cout<<"\t\t\t |===========================|\t\t\t"<<endl;
			cout<<"\t\t\t  Pilihan Anda = "; cin>>tipe;
			if (tipe==1)
			{
				system("cls");
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t |----------------Spesifikasi Iphone X-----------------|"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : Dual 12 MP \t\t\t"<<endl;
				cout<<"\t\t\t   Kamera Depan : 7 MP "<<endl;
				cout<<"\t\t\t   Memory : No Card Slot, Internal 64/256 GB, 3 GB RAM"<<endl;
				cout<<"\t\t\t   Sistem Operasi : iOS 11.1.1, upgradable to iOS 12.1"<<endl;
				cout<<"\t\t\t   CPU : Hexa-core 2.39 GHz (2x Monsoon + 4x Mistral)"<<endl;
				cout<<"\t\t\t   Baterai : Non-removable Li-Ion 2716 mAh battery (10.35 Wh)"<<endl;
				cout<<"\t\t\t   Ukuran : 5.8 inches"<<endl;
				cout<<"\t\t\t   Jaringan : GSM/HSPA/LTE"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.10.900.000"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
			}
			if (tipe==2)
			{
				system("cls");
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t |----------------Spesifikasi Iphone 8-----------------|"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : 12 MP "<<endl;
				cout<<"\t\t\t   Kamera Depan : 7 MP "<<endl;
				cout<<"\t\t\t   Memory : No Card Slot, Internal 64/256 GB, 2 GB RAM"<<endl;
				cout<<"\t\t\t   Sistem Operasi : iOS 11.1.1, upgradable to iOS 12.1"<<endl;
				cout<<"\t\t\t   CPU : Hexa-core 2.39 GHz (2x Monsoon + 4x Mistral)"<<endl;
				cout<<"\t\t\t   Baterai : Non-removable Li-Ion 1821 mAh battery"<<endl;
				cout<<"\t\t\t   Ukuran : 4.7 inches"<<endl;
				cout<<"\t\t\t   Jaringan : GSM/HSPA/LTE"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.7.200.000"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
			}
		}
		if (merk==2)
		{
			cout<<"\t\t\t |============================|\t\t\t"<<endl;
			cout<<"\t\t\t |--Pilih Jenis Tipe Samsung--|\t\t\t"<<endl;
			cout<<"\t\t\t |-----1. SAMSUNG S9-----=----|\t\t\t"<<endl;
			cout<<"\t\t\t |-----2. SAMSUNG NOTE 9------|\t\t\t"<<endl;
			cout<<"\t\t\t |===========================|\t\t\t"<<endl;
			cout<<"\t\t\t  Pilihan Anda = "; cin>>tipe;
			if (tipe==2)
			{
				system("cls");
				cout<<"\t\t\t |=======================================================|"<<endl;
				cout<<"\t\t\t |----------------Spesifikasi Samsung S9-----------------|"<<endl;
				cout<<"\t\t\t |=======================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : 12 MP "<<endl;
				cout<<"\t\t\t   Kamera Depan : 8 MP "<<endl;
				cout<<"\t\t\t   Memory : microSD upto 512 GB, 64/128/256 GB, 4 GB RAM"<<endl;
				cout<<"\t\t\t   Sistem Operasi : Android 8.0 (Oreo)"<<endl;
				cout<<"\t\t\t   CPU : Octa-core"<<endl;
				cout<<"\t\t\t   Baterai : Non-removable Li-Ion 3000 mAh battery"<<endl;
				cout<<"\t\t\t   Ukuran : 5.8 inches"<<endl;
				cout<<"\t\t\t   Jaringan : GSM//CDMA/HSPA/EVDO/LTE"<<endl;
				cout<<"\t\t\t |=======================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.8.990.000"<<endl;
				cout<<"\t\t\t |=======================================================|"<<endl;
			}
			if (tipe==3)
			{
				system("cls");
				cout<<"\t\t\t |===========================================================|"<<endl;
				cout<<"\t\t\t |----------------Spesifikasi Samsung NOTE 9-----------------|"<<endl;
				cout<<"\t\t\t |===========================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : 12 MP "<<endl;
				cout<<"\t\t\t   Kamera Depan : 8 MP "<<endl;
				cout<<"\t\t\t   Memory : microSD upto 512 GB, 512 GB, 8 GB RAM or 128 GB"<<endl;
				cout<<"\t\t\t   Sistem Operasi :  Android 8.0 (Oreo)"<<endl;
				cout<<"\t\t\t   CPU : Hexa-core 2.39 GHz (2x Monsoon + 4x Mistral)"<<endl;
				cout<<"\t\t\t   Baterai : Non-removable Li-Ion 4000 mAh battery"<<endl;
				cout<<"\t\t\t   Ukuran : 6.4 inches"<<endl;
				cout<<"\t\t\t   Jaringan : GSM//CDMA/HSPA/EVDO/LTE"<<endl;
				cout<<"\t\t\t |===========================================================|"<<endl;
				cout<<"Harga = Rp.9.750.000"<<endl;
				cout<<"\t\t\t |===========================================================|"<<endl;
			}
		}
		
	}
	if (spek==2)
	{
		cout<<"\t\t\t |============================================|\t\t\t"<<endl;
		cout<<"\t\t\t |--Pilih Merk Smartphone Spesifikasi Rendah--|\t\t\t"<<endl;
		cout<<"\t\t\t |-----------------1. IPHONE------------------|\t\t\t"<<endl;
		cout<<"\t\t\t |-----------------2. SAMSUNG-----------------|\t\t\t"<<endl;
		cout<<"\t\t\t |============================================|\t\t\t"<<endl;
		cout<<"\t\t\t  Pilihan Anda = "; cin>>merk;
		if (merk==1)
		{
			cout<<"\t\t\t |===========================|\t\t\t"<<endl;
			cout<<"\t\t\t |--Pilih Jenis Tipe Iphone--|\t\t\t"<<endl;
			cout<<"\t\t\t |-------1. IPHONE 5S---------|\t\t\t"<<endl;
			cout<<"\t\t\t |-------2. IPHONE 5---------|\t\t\t"<<endl;
			cout<<"\t\t\t |===========================|\t\t\t"<<endl;
			cout<<"\t\t\t  Pilihan Anda = "; cin>>tipe;
			if (tipe==1)
			{
				system("cls");
				cout<<"\t\t\t |======================================================|"<<endl;
				cout<<"\t\t\t |----------------Spesifikasi Iphone 5s-----------------|"<<endl;
				cout<<"\t\t\t |======================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : Dual 12 MP "<<endl;
				cout<<"\t\t\t   Kamera Depan : 7 MP "<<endl;
				cout<<"\t\t\t   Memory : No Card Slot, Internal 64/256 GB, 3 GB RAM"<<endl;
				cout<<"\t\t\t   Sistem Operasi : iOS 11.1.1, upgradable to iOS 12.1"<<endl;
				cout<<"\t\t\t   CPU : Hexa-core 2.39 GHz (2x Monsoon + 4x Mistral)"<<endl;
				cout<<"\t\t\t   Baterai : Non-removable Li-Ion 2716 mAh battery "<<endl;
				cout<<"\t\t\t   Ukuran : 5.8 inches"<<endl;
				cout<<"\t\t\t   Jaringan : GSM/HSPA/LTE"<<endl;
				cout<<"\t\t\t |======================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.1.500.000"<<endl;
				cout<<"\t\t\t |======================================================|"<<endl;
			}
			if (tipe==2)
			{
				system("cls");
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t |----------------Spesifikasi Iphone 5-----------------|"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : Dual 12 MP "<<endl;
				cout<<"\t\t\t   Kamera Depan : 7 MP "<<endl;
				cout<<"\t\t\t   Memory : No Card Slot, Internal 64/256 GB, 3 GB RAM"<<endl;
				cout<<"\t\t\t   Sistem Operasi : iOS 11.1.1, upgradable to iOS 12.1"<<endl;
				cout<<"\t\t\t   CPU : Hexa-core 2.39 GHz (2x Monsoon + 4x Mistral)"<<endl;
				cout<<"\t\t\t   Baterai : Non-removable Li-Ion 2716 mAh battery"<<endl;
				cout<<"\t\t\t   Ukuran : 5.8 inches"<<endl;
				cout<<"\t\t\t   Jaringan : GSM/HSPA/LTE"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.1.200.000"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
			}
		}
		if (merk==2)
		{
			cout<<"\t\t\t |============================|\t\t\t"<<endl;
			cout<<"\t\t\t |--Pilih Jenis Tipe Samsung--|\t\t\t"<<endl;
			cout<<"\t\t\t |-------1. SAMSUNG j5--------|\t\t\t"<<endl;
			cout<<"\t\t\t |-------2. IPHONE j2---------|\t\t\t"<<endl;
			cout<<"\t\t\t |============================|\t\t\t"<<endl;
			cout<<"\t\t\t  Pilihan Anda = "; cin>>tipe;
			if (tipe==1)
			{
				system("cls");
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t |-----------Spesifikasi Samsung Galaxy J5-------------|"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : 13 MP, f/1.9, 28mm (wide), AF "<<endl;
				cout<<"\t\t\t   Kamera Depan : 	5 MP, f/2.2, 23mm (wide)"<<endl;
				cout<<"\t\t\t   Memory : 8/16 GB, 1.5 GB RAM, microSD, up to 256 GB"<<endl;
				cout<<"\t\t\t   Sistem Operasi : Android 5.1 (Lollipop)"<<endl;
				cout<<"\t\t\t   CPU : Quad-core 1.2 GHz Cortex-A53"<<endl;
				cout<<"\t\t\t   Baterai : Removable Li-Ion 2600 mAh battery"<<endl;
				cout<<"\t\t\t   Ukuran : 5.0 inches, 68.9 cm2"<<endl;
				cout<<"\t\t\t   Jaringan : GSM/HSPA/LTE"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.1.300.000"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
			}
			if (tipe==2)
			{
				system("cls");
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t |-----------Spesifikasi Samsung Galaxy J2-------------|"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Kamera Utama : 5 MP, AF, f/2.2"<<endl;
				cout<<"\t\t\t   Kamera Depan : 	2 MP, f/2.2"<<endl;
				cout<<"\t\t\t   Memory :8 GB, 1 GB RAM, microSD, up to 256 GB"<<endl;
				cout<<"\t\t\t   Sistem Operasi : Android 5.1 (Lollipop)"<<endl;
				cout<<"\t\t\t   CPU : Quad-core 1.3 GHz Cortex-A7"<<endl;
				cout<<"\t\t\t   Baterai : Removable Li-Ion 2000 mAh battery"<<endl;
				cout<<"\t\t\t   Ukuran : 4.7 inches, 60.9 cm2 (~64.7% screen-to-body ratio)"<<endl;
				cout<<"\t\t\t   Jaringan : GSM/HSPA/LTE"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
				cout<<"\t\t\t   Harga = Rp.1.050.000"<<endl;
				cout<<"\t\t\t |=====================================================|"<<endl;
			}
		}
	}   
		cout<<"\t\t\t   Ingin Membeli \n\t\t\t   1. Ya \t 2. Tidak \n\t\t\t   --1/2--: "; cin>>beli;
		if (beli==1)
		{
			cout<<"\t\t\t |==========================================================|"<<endl;
			cout<<"\t\t\t |----------------SMARTPHONE CELLER CENTER GOWA-------------|"<<endl;
			cout<<"\t\t\t |==========================================================|"<<endl;
    		cout<<"\t\t\t   Masukkan Nama : "; cin>>tmp.data.nama;
   		 	cout<<"\t\t\t   Masukkan Alamat : "; cin>>tmp.data.alamat;
   			cout<<"\t\t\t   Masukkan Nomor HAPE :"; cin>>tmp.data.nope;
			cout<<"\t\t\t   Smartphone Yang anda Pilih : "; cin>>tmp.data.phone; 
			cout<<"\t\t\t   Masukkan Harga Smartphone : Rp"; cin>>tmp.data.harga;
			cout<<"\t\t\t   Jumlah Uang Pembayaran = Rp"; cin>>tmp.data.bayar;
			tmp.data.kembali=tmp.data.bayar-tmp.data.harga;
			cout<<"\t\t\t   Uang Kembalian = Rp"<<tmp.data.kembali<<endl;
			input(tmp.data);
			cout<<"\t\t\t |==========================================================|\t\t\t"<<endl;
		}
		else if (beli==2)
		{
			cout<<"\t\t\t |==========================================================|"<<endl;
			cout<<"\t\t\t |----------------SMARTPHONE CELLER CENTER GOWA-------------|"<<endl;
			cout<<"\t\t\t |==========================================================|"<<endl;
			cout<<"\t\t\t |-------------TERIMA KASIH, TABUNG UANGNYA DULU :)---------|"<<endl;
			cout<<"\t\t\t |==========================================================|"<<endl;
		}   
			break;
      case '2' :
            hapuss();
            break;
      case '3' :
            cetak();
            break;
      case '4' :
            exit(0);
            break;
      default :
            cout<<"\n\t\t\t   Pilihan salah"<<endl;
      }
      cout<<"\t\t\t   Kembali ke menu?(y/n) : ";
      cin>>ulang;
   	}
	   while(ulang=='y' || ulang=='Y');

      return EXIT_SUCCESS;
}

