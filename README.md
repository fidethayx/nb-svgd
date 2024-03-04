# nb-svgd#include <stdio.h>
#include <conio.h>

struct sv
{
	char maso[10];
	char ht[25];
	float dtb;
};

void main()
{
	int i, n;
	float d;
	sv bg;
	FILE * f;
	clrscr();
	f = fopen("HosoSV.DAT", "w+b");
	printf("Nhap so sv n=");
	scanf("%d", &n);
	fwrite(&n, sizeof(int), 1, f);
	for (i = 1; i <= n; i++)
	clrscr();
	gotoxy(10, 1);
	printf("Danh sach sinh vien\n\n");
	printf("%-10s%-25s%-10s\n\n", "Ma so", "Ho va ten#include <stdio.h>
#include <conio.h>

struct sv
{
	char maso[10];
	char ht[25];
	float dtb;
};

void main()
{
	int i, n;
	float d;
	sv bg;
	FILE * f;
	clrscr();
	f = fopen("HosoSV.DAT", "w+b");
	printf("Nhap so sv n=");
	scanf("%d", &n);
	fwrite(&n, sizeof(int), 1, f);
	for (i = 1; i <= n; i++)
	{
		printf("nhap du lieu cua sv thu %d :\n", i);
		fflush(stdin);
		printf("Ma so : ");
		gets(bg.maso);
		printf("Ho va ten : ");
		gets(bg.ht);
		printf("Diem TB : ");
		scanf("%f", &d);
		bg.dtb = d;
		fwrite(&bg, sizeof(sv), 1, f);
	}

{
	char i, s[30];
	FILE * f;
	clrscr();
	f = fopen("DSSV.TXT", "w");
	i = 1;
	printf("Nhap ho ten cua tung hoc sinh, ket thuc go Enter\n");
	do {
		printf("Ho ten hoc sinh thu %d : ", i++);
		gets(s);
		if (strlen(s) > 0)
		{
			strcat(s, "\n");
			fputs(s, f);
		}
	} while (strlen(s) > 0);
	fclose(f);
	clrscr();
	fclose(f);
	f = fopen("HosoSV.DAT", "rb");
	fread(&n, sizeof(int), 1, f);
	clrscr();
	gotoxy(10, 1);
	printf("Danh sach sinh vien\n\n");
	printf("%-10s%-25s%-10s\n\n", "Ma so", "Ho va ten", "Diem TB");
	for (i = 1; i <= n; i++)
	{
		fread(&bg, sizeof(sv), 1, f);
{
	char i, s[30];
	FILE * f;
	clrscr();
	f = fopen("DSSV.TXT", "w");
	i = 1;
	printf("Nhap ho ten cua tung hoc sinh, ket thuc go Enter\n");
	do {
		printf("Ho ten hoc sinh thu %d : ", i++);
		gets(s);
		if (strlen(s) > 0)
		{
			strcat(s, "\n");
			fputs(s, f);
		}
	} while (strlen(s) > 0);
	fclose(f);
	clrscr();
		printf("%-10s%-25s%-10.1f\n", bg.maso, bg.ht, bg.dtb);
	}

	fclose(f);
	printf("\nGo Enter ket thuc ...");
{
	char i, s[30];
	FILE * f;
	clrscr();
	f = fopen("DSSV.TXT", "w");
	i = 1;
	printf("Nhap ho ten cua tung hoc sinh, ket thuc go Enter\n");
	do {
		printf("Ho ten hoc sinh thu %d : ", i++);
		gets(s);
		if (strlen(s) > 0)
		{
			strcat(s, "\n");
			fputs(s, f);
		}
	} while (strlen(s) > 0);
	fclose(f);
	clrscr();
	getch();
}", "Diem TB");
	for (i = 1; i <= n; i++)
	{
		fread(&bg, sizeof(sv), 1, f);
		printf("%-10s%-25s%-10.1f\n", bg.maso, bg.ht, bg.dtb);
	}

	fclose(f);
	printf("\nGo Enter ket thuc ...");
	getch();
}
