```cpp
#include <iostream>
using namespace std;
int main(){
    while (true){
        srand(time(NULL));
        int rl = rand() % 7, rr = rand() % 7;
        int x = rand() % 50 + 5;
        int count = 0;
        bool player_turn = true;
        bool boom = false;
        cout << "歡迎來到定時炸彈的遊戲，炸彈會在一個範圍內，你和電腦會比看誰先數到炸彈，輸入0000結束遊戲";
        while (count <= x){
            cout << endl << "炸彈介於" << x - rl<< "~" << x + rr << endl;
            cout << "目前數字為:" << count << endl;
            if (player_turn){
                int input;
                cout << "輸入1~3的整數:";
                cin >> input;
                if (input == 0000){
                    cout << "結束遊戲" << endl;
                    return 0;
                }
                if (input >= 1 && input <= 3){
                    count += input;
                    player_turn = false;
                }
                else{
                    cout << "輸入錯誤，再輸一次" << endl;
                }
            }
            else{
                int random = rand() % 3 + 1;
                cout << "電腦輸入:" << random << endl;
                count += random;
                player_turn = true;
            }
            if (count == x){
                boom = true;
            }
        }
        if (boom){
            if (player_turn){
                cout << "你贏了" << endl;
            }
            else{
                cout << "你輸了" << endl;
            }
        }
        else{
            cout << "安全度過" << endl;
        }
        cout << "數字為:" << x << endl;
    }
}
```
