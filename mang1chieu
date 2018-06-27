#include <iostream>
#include <cstdlib>
#include <ctime>
#define MAX 1000

using namespace std;

void nhapMang(int arr[], int &n)
{
	srand(time(NULL));
	cout << "nhap so phan tu vao mang: ";
	cin >> n;
	for (int i = 0; i < n; i++)
	{
		arr[i] = rand() % 100 + 1;
	}
}

void xuatMang(int arr[], int n)
{
	for (int i = 0; i < n; i++)
	{
		cout << "arr[" << i << "]: " << arr[i] << endl;
	}
	
}

void saoChepMang(int mangDich[], int mangNguon[], int n)
{
	for (int i = 0; i < n; i++)
	{
		mangDich[i] = mangNguon[i];
	}
}

int timKiem(int arr[], int n, int x)
{
	for (int i = 0; i < n; i++)
	{
		if (arr[i] == x)
		{
			cout << "o mang so " << i << endl;
			return i;
		}
	}
		return -1;
	
}

void hoanvi(int &a, int &b)
{
	int temp = a;
	a = b;
	b = temp;

}

void soSanh(int arr[], int n)
{
	for (int i = 0; i < n-1; i++)
	{
		for (int j = i+1; j < n; j++)
		{
			if (arr[i] > arr[j])
				hoanvi(arr[i], arr[j]);
		}

	}
}

void themGiaTri(int arr[], int &n, int idx,int x)
{
	if ((idx >= 0) && (idx <= n))
	{
		for (int i = n; i > idx; i--)
			arr[i] = arr[i - 1];
		arr[idx] = x;
		n++;
	}
	
}

void xoaGiaTri(int a[], int &n, int idx)
{
	if (idx >= 0 && idx <= n)
	{
		for (int i = idx; i < n-1; i++)
		{
			a[i] = a[i + 1];
		}
		n--;

	}

}
int main()
{
	int myArray[MAX];
	int nSize;
	
	nhapMang(myArray, nSize);
	xuatMang(myArray, nSize);

	cout << "nhap gia tri can them: ";
	int x;
	cin >> x;

	cout << "vi tri can them: ";
	int idx;
	cin >> idx;
	
	themGiaTri(myArray, nSize, idx, x);
	xuatMang(myArray, nSize);
	
	cout << "vi tri can xoa: ";
	int idx1;
	cin >> idx1;
	cout<<"ngo the sonaaaaaaaa";
	xoaGiaTri(myArray, nSize, idx1);
	
	xuatMang(myArray, nSize);

	system("pause");
	return 0;
}
