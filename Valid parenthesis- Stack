#include <iostream>
#include <stack>
using namespace std;

bool isValidParenthesis(const string& S) {
    stack<char> stk;

    for (char c : S) {
        if (c == '(') {
            stk.push(c);
        } else if (c == ')') {
            if (!stk.empty() && stk.top() == '(') {
                stk.pop();
            } else {
                return false;
            }
        }
    }
    return stk.empty();
}

int main() {
    int T;
    cin >> T;
    while (T--) {
        string S;
        cin >> S;
        cout << (isValidParenthesis(S) ? 1 : 0) << endl;
    }
    return 0;
}
