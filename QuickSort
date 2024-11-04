#include <stdio.h>
void quickSort(int arr[], int first, int last) {
if (first < last) {
int pivot = arr[first];
int i = first + 1;

for (int j = first + 1; j <= last; j++) {
if (arr[j] < pivot) {
int temp = arr[i];
arr[i] = arr[j];
arr[j] = temp;
i++;
}
}

int temp = arr[first];
arr[first] = arr[i - 1];
arr[i - 1] = temp;

int pivotIndex = i - 1;

quickSort(arr, first, pivotIndex - 1);
quickSort(arr, pivotIndex + 1, last);
}
}

int main() {
int n;
printf("Enter the number of elements: ");
scanf("%d", &n);

int arr[n];
printf("Enter %d elements:\n", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
}

quickSort(arr, 0, n - 1);

printf("Sorted array:\n");
for (int i = 0; i < n; i++) {
printf("%d ", arr[i]);
}
printf("\n");

return 0;
}
