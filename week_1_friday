#include <iostream>

int findSecondLargest(int arr[], int n) {
  if (n < 2) {
    return -1;
  }

  int largest = arr[0];
  int secondLargest = -1;

  for (int i = 1; i < n; i++) {
    if (arr[i] > largest) {
      largest = arr[i];
    }
  }

  for (int i = 0; i < n; i++) {
    if (arr[i] > secondLargest && arr[i] < largest) {
      secondLargest = arr[i];
    }
  }

  return secondLargest;
}

int main() {
  int arr[] = {12, 35, 1, 10, 34, 1};
  int n = sizeof(arr) / sizeof(arr[0]);

  int secondLargest = findSecondLargest(arr, n);

  if (secondLargest == -1) {
    std::cout << "Array has less than two elements." << std::endl;
  } else {
    std::cout << "The second largest element is: " << secondLargest << std::endl;
  }

  return 0;
}
