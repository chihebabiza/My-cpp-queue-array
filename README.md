# Queue Implementation Using Dynamic Array in C++

A simple, template-based queue class in C++ built on top of a custom dynamic array (`clsDynamicArray`). This implementation supports core queue operations such as `push`, `pop`, `front`, and `back`, along with extended utilities like reversing the queue and inserting at custom positions.

---

## 📦 Features

- FIFO Queue behavior (`push` to back, `pop` from front)
- Supports any data type via templates
- View the front and back elements
- Get size or check if queue is empty
- Insert items at the front, back, or after a specific index
- Reverse the queue
- Update items by index
- Clear all contents

---

## 🧪 Example Usage

```cpp
#include <iostream>
#include "clsMyQueueArr.h"

int main() {
    clsMyQueueArr<int> myQueue;

    myQueue.push(10);
    myQueue.push(20);
    myQueue.push(30);

    cout << "Front: " << myQueue.front() << endl; // 10
    cout << "Back: " << myQueue.back() << endl;   // 30

    myQueue.pop();  // removes 10
    myQueue.Print(); // Output: 20 30

    myQueue.InsertAfter(0, 25);
    myQueue.UpdateItem(1, 22);
    myQueue.Print(); // Output: 20 22 30

    myQueue.Reverse();
    myQueue.Print(); // Output: 30 22 20
}
````

---

## 📘 Public Methods

| Method                      | Description                   |
| --------------------------- | ----------------------------- |
| `push(value)`               | Add item to back of the queue |
| `pop()`                     | Remove item from front        |
| `front()`                   | Return front element          |
| `back()`                    | Return back element           |
| `Print()`                   | Display all queue elements    |
| `Size()`                    | Return number of elements     |
| `IsEmpty()`                 | Check if queue is empty       |
| `GetItem(index)`            | Get element at index          |
| `UpdateItem(index, value)`  | Update value at index         |
| `InsertAfter(index, value)` | Insert after a given index    |
| `InsertAtFront(value)`      | Insert item at the front      |
| `InsertAtBack(value)`       | Insert item at the back       |
| `Reverse()`                 | Reverse queue order           |
| `Clear()`                   | Clear all elements            |

---

## 🔧 Dependencies

* Requires `clsDynamicArray.h` (your custom dynamic array class)

Make sure to include both `.h` files and use `#include "clsMyQueueArr.h"` in your project.

---

## 📚 Use Case

Ideal for:

* Teaching data structures
* Simple queue logic in C++
* Practicing dynamic memory and templates

---

## 🧾 License

This project is provided under the MIT License. See [LICENSE](LICENSE.txt) for details.


