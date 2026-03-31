#include <stdio.h>

int main() {
    float p, r, t, SI, CI, amount;
    int i;
    printf("Enter Principal amount: ");
    scanf("%f", &p);
    printf("Enter Rate of interest: ");
    scanf("%f", &r);
    printf("Enter Time (in years): ");
    scanf("%f", &t);
    SI = (p * r * t) / 100;
    amount = p;
    for(i = 1; i <= t; i++) {
        amount = amount * (1 + r / 100);
    }
    CI = amount - p;
    printf("\nSimple Interest = %.2f", SI);
    printf("\nCompound Interest = %.2f", CI);
     return 0;
}
