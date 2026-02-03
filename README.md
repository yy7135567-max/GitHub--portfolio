#include <iostream>
using namespace std;

class Student {
    int roll;

public:
    Student(int r) {
        roll = r;
    }

    Student(Student &s) {
        roll = s.roll;
    }

    void show() {
        cout << roll << endl;
    }
};

int main() {
    Student s1(10);
    Student s2 = s1;
    s2.show();
    return 0;
}