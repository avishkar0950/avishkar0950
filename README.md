#include <iostream>
#include <stack>
#include <queue>

using namespace std;

// Function to perform stack operations
void operateStack(stack<int>& myStack) {
    // Push elements into the stack
    myStack.push(1);
    myStack.push(2);
    myStack.push(3);

    // Pop elements from the stack
    while (!myStack.empty()) {
        cout << "Stack top: " << myStack.top() << endl;
        myStack.pop();
    }
}

// Function to perform queue operations
void operateQueue(queue<int>& myQueue) {
    // Push elements into the queue
    myQueue.push(1);
    myQueue.push(2);
    myQueue.push(3);

    // Pop elements from the queue
    while (!myQueue.empty()) {
        cout << "Queue front: " << myQueue.front() << endl;
        myQueue.pop();
    }
}

int main() {
    // Stack
    stack<int> myStack;
    operateStack(myStack);

    // Queue
    queue<int> myQueue;
    operateQueue(myQueue);

    return 0;
}
