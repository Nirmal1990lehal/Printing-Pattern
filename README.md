#include <stdio.h>
int main() {
  int n, i, k, b, a, p, q;
  scanf("%d", &n);
  for (i = 0; i <= 2 * n - 2; i++) {
    printf("%d ", n);
  }
  printf("\n");
  p = n;
  for (i = 0; i < n - 1; i++) {
    a = 0;
    for (k = 0; k <= i; k++) {
      printf("%d ", n - a);
      a++;
    }
    for (b = 0; b > i; b++) {
      printf("   ");
    }
    for (k = 1; k <= 2 * p - 3; k++) {
      printf("%d ", n - i - 1);
    }
    p--;
    for (k = i; k >= 0; k--) {
      printf("%d ", n - k);
    }
    printf("\n");
  }
  q = 1;
  for (i = 0; i < n - 2; i++) {
    for (k = n; k > i + 1; k--) {
      printf("%d ", k);
    }
    for (k = 1; k < 2 * q + 0; k++) {
      printf("%d ", q + 1);
    }
    ++q;
    for (k = 2 + i; k <= n; k++) {
      printf("%d ", k);
    }
    printf("\n");
  }
  for (i = 0; i < 2 * n - 1; i++) {
    printf("%d ", n);
  }
  return 0;
}
