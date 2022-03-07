#include <bits/stdc++.h>
using namespace std;

int main()
{
    long long n, money, s(0);
    cin >> n >> money;
    long long lst[n]{};
    for (int i = 0; i < n; i++)
    {
        cin >> lst[i];
    }
    for (int i = 0; i < n - 1; i++)
    {
        for (int x = i + 1; x < n; x++)
        {
            if (lst[i] + lst[x] == money)
            {
                s++;
            }
        }
    }
    cout << s << endl;
    return 0;
}
