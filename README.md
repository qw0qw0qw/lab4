# Lab4. Домашняя работа

# Условия задачи
Друзья заказали пиццу. Они решат, резать ее на 4 или 6 кусков, по простому правилу: если ровно один из них (Ваня A или Петя B) проголодался (его "уровень голода" - четное число), то резать на 4 части. Запишите условие для нарезки на 4 части.

# Блоксхема
<img width="221" height="771" alt="lab4" src="https://github.com/user-attachments/assets/239bb6eb-9322-4128-904c-66bea17adb1c" />

# Реализация программы

```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <locale.h>

int main() {
	setlocale(LC_CTYPE, "RUS");
	int a;
	int b;

	puts("Введите уровень голода Пети и Вани: ");
	scanf("%d %d", &a, &b);

	int res = (a + b) % 2;
	printf("1 - Резать на 6 частей \n0 - Резать на 4 части \nВаш результат: %d", res);
}
```

# Результат программы

<img width="345" height="175" alt="image" src="https://github.com/user-attachments/assets/7894cc3c-3fb2-4023-9d03-3ae26e4685e3" />
