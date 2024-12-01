# c-
New for C++ Developers in Visual Studio 2022
#include <iostream>
#include <ranges>
#include <vector>

int main() {
    std::vector<int> numbers = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

    // Filter and transform using ranges
    auto result = numbers 
        | std::views::filter([](int n) { return n % 2 == 0; }) 
        | std::views::transform([](int n) { return n * n; });

    std::cout << "Even squares: ";
    for (int n : result) {
        std::cout << n << " ";
    }

    return 0;
    https://www.skntechnology.in
    
}
