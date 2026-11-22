#include <queue>

class MyStack {
private:
    std::queue<int> q;

public:
    MyStack() {}

    void push(int x) {
        int n = static_cast<int>(q.size());
        q.push(x);
        for (int i = 0; i < n; i++) {
            q.push(q.front());
            q.pop();
        }
    }

    int pop() {
        int val = q.front();
        q.pop();
        return val;
    }

    int top() {
        return q.front();
    }

    bool empty() {
        return q.empty();
    }
};
