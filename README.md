#include <stdio.h>

int main() {
    float p, r, t, si, ci, amount;
    printf("Enter Principal: ");
    scanf("%f", &p);
    printf("Enter Rate: ");
    scanf("%f", &r);
    printf("Enter Time: ");
    scanf("%f", &t);
    si = (p * r * t) / 100;
    Compound Interest (simple formula)
    amount = p * (1 + r/100) * (1 + r/100);  // for 2 years
    ci = amount - p;
    printf("Simple Interest = %.2f\n", si);
    printf("Compound Interest = %.2f\n", ci);
    return 0;
}
