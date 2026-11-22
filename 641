class MyCircularDeque {
private:
    vector<int> buf;
    int cap;
    int front;
    int size;

public:
    MyCircularDeque(int k) : buf(k, 0), cap(k), front(0), size(0) {}

    bool insertFront(int value) {
        if (isFull()) {
            return false;
        }
        front = (front - 1 + cap) % cap;
        buf[front] = value;
        ++size;
        return true;
    }

    bool insertLast(int value) {
        if (isFull()) {
            return false;
        }
        int rear = (front + size) % cap;
        buf[rear] = value;
        ++size;
        return true;
    }

    bool deleteFront() {
        if (isEmpty()) {
            return false;
        }
        front = (front + 1) % cap;
        --size;
        return true;
    }

    bool deleteLast() {
        if (isEmpty()) {
            return false;
        }
        --size;
        return true;
    }

    int getFront() {
        if (isEmpty()) {
            return -1;
        }
        return buf[front];
    }

    int getRear() {
        if (isEmpty()) {
            return -1;
        }
        int rear = (front + size - 1) % cap;
        return buf[rear];
    }

    bool isEmpty() {
        return size == 0;
    }

    bool isFull() {
        return size == cap;
    }
};
