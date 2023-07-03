# -4
Натуральне число m називається рівним дільником числа n, якщо частка і залишок від ділення n на m дорівнюють одне одному. Для заданого натурального числа n знайти кількість його рівних дільників.

#include <stdio.h>

int main() {

unsigned int n;

printf("Enter a natural number n: ");

scanf("%u", &n);
unsigned int count = 0;

for (unsigned int m = 1; m <= n; m++) {
        
if (n % m == n / m) {
            count = count +

1;
        }
    }

printf("The number of equal divisors of a number %u: %u\n", n, count);

return 0;
}
