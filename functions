#include <iostream>
#include <string>
#include <sstream>
#include<map>

int sumLastNums (int x)
{
    int z = x % 10 + x % 100 / 10;
    return z;
}

bool isPositive (int x)
{

    if (x > 0)
        return true;
    else
        return false;
}

bool isUpperCase (char x)
{
    char alf[] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z'};
    
    for(int i {1}; i < 27; i++)
    {
        if (x == alf[i-1])
            return true;
    }
    return false;
}

bool isDivisor (int a, int b)
{
    if (a % b == 0)
        return true;
    else if (b % a == 0)
        return true;
    else 
        return false;
}

int lastNumSum(int a, int b)
{
    return (a % 10 + b % 10);
}

double safeDiv (int a, int b)
{
    if (b == 0)
        return 0;
    else
        return (a / b);
}

std::string makeDecision (int x, int y)
{
    std::stringstream ss;
    if (x > y)
    {
        ss << x;
        std::string s_x = ss.str();
        ss.str(std::string());
        ss << y;
        std::string y_x = ss.str();
        std::string s = s_x + '>' + y_x;
        return s;
    }
    else if (x < y)
    {
        ss << x;
        std::string s_x = ss.str();
        ss.str(std::string());
        ss << y;
        std::string y_x = ss.str();
        std::string s = s_x + '<' + y_x;
        return s;
    }
    else 
    {
        ss << x;
        std::string s_x = ss.str();
        ss.str(std::string());
        ss << y;
        std::string y_x = ss.str();
        std::string s = s_x + '=' + '=' + y_x;
        return s; 
    }
}

bool sum3 (int x, int y, int z)
{
    if (x + y == z)
        return true;
    else if (x + z == y)
        return true;
    else if (y + z == x)
        return true;
    else
        return false;
}

std::string age (int x)
{
    std::stringstream ss;

    if (x % 10 == 1 && x != 11)
    {
        ss << x;
        std::string s_x = ss.str();
        std::string s = s_x + " год";
        return s;
    }
    else if ((x != 12 && x % 10 == 2)||(x != 13 && x % 10 == 3) || (x % 10 == 4 && x != 14))
    {
        ss << x;
        std::string s_x = ss.str();
        std::string s = s_x + " года";
        return s;
    }
    else
    {
        ss << x;
        std::string s_x = ss.str();
        std::string s = s_x + " лет";
        return s;
    }
}

void printDays (std::string x)
{
    std::map <std::string, int> mapping;
    mapping["понедельник"] = 1;
    mapping["вторник"] = 2;
    mapping["среда"] = 3;
    mapping["четверг"] = 4;
    mapping["пятница"] = 5;
    mapping["суббота"] = 6;
    mapping["воскресение"] = 7;
    switch(mapping[x])
    {
        case 1:
            std::cout << "понедельник" << "\n";
        case 2:
            std::cout << "вторник" << "\n";
        case 3:
            std::cout << "среда" << "\n";
        case 4:
            std::cout << "четверг" << "\n";
        case 5:
            std::cout << "пятница" << "\n";
        case 6:
            std::cout << "суббота" << "\n";
        case 7:
            std::cout << "воскресение" << "\n";
            break;
        default:
            std::cout << "это не день недели";
    }
}

std::string reverseListNums (int x)
{
    std::stringstream ss;
    ss << x;
    std::string s = ss.str();
    ss.str(std::string());
    for(int i {x-1}; i != -1; i--)
    {
        ss << i;
        s = s + " " + ss.str();
        ss.str(std::string());
    }
    return s;
}

int pow (int x, int y)
{
    int new_x = x;
    for(int i {y}; i != 1; i--)
    {
        new_x = new_x * x;
    }
    return new_x;
}

bool equalNum (int x)
{
    if ((x < 10 &&  x > 0) || (x < 0 && x > -10))
        return false;
    int check_x = x % 10;
    while(x > 1 || x < -1)
    {
        if (check_x != x % 10)
            return false;
        x = x / 10;
    }
    return true;
}

void leftTriangle (int x)
{
    std::string trio = "*";
    for(int i {0}; i < x; i++)
    {
        std::cout<<trio<<"\n";
        trio += "*";
    }
}

int main() {
    std::cout<<"Выберите функцию для выполнения \n sumLastNums -- 1 \n isPositive -- 2 \n isUpperCase -- 3\n isDivisor -- 4 \n safeDiv -- 5 \n makeDecision -- 6\n sum3 -- 7\n string age -- 8\n printDays -- 9 \n reverseListNums -- 10 \n pow -- 11 \n equalNum -- 12 \n leftTriangle -- 13 \n";
    int choice;
    std::cin>>choice;
    
    switch(choice)
    {
        case 1:
            int sumLastNums_x;
            std::cout<<"Введитие число. Функция вернет результат сложения двух полседних цифр \n";
            std::cin>>sumLastNums_x;
            std::cout<<"Ответ -- "<<sumLastNums(sumLastNums_x);
            break;
        
        case 2:
            int isPositive_x;
            std::cout<<"Введитие число. Функция выведет true если число положительное \n";
            std::cin>>isPositive_x;
            std::cout<<"Ответ -- "<<std::boolalpha<<isPositive(isPositive_x);
            break;
        
        case 3:
            char isUpperCase_x;
            std::cout<<"Введитие букву. Функция выведет true если буква большая латинская \n";
            std::cin>>isUpperCase_x;
            std::cout<<"Ответ -- "<<std::boolalpha<<isUpperCase(isUpperCase_x);
            break;
        
        case 4:
            int isDivisor_x,isDivisor_y;
            std::cout<<"Введитие два числа. Функция выведет true если одно из чисел можно поделить на другое \n";
            std::cin>>isDivisor_x>>isDivisor_y;
            std::cout<<"Ответ -- "<<std::boolalpha<<isDivisor(isDivisor_x,isDivisor_y);
            break;
        
        case 5:
            int safeDiv_x,safeDiv_y;
            std::cout<<"Введитие  два числа. Функция безопасно разделит с учетом невозмножности деления на 0  \n";
            std::cin>>safeDiv_x>>safeDiv_y;
            std::cout<<"Ответ -- "<<safeDiv(safeDiv_x,safeDiv_y);
            break;
        
        case 6:
            int makeDecision_x,makeDecision_y;
            std::cout<<"Введитие два числа. Функция вернет эти числа со знаком > < = \n";
            std::cin>>makeDecision_x>>makeDecision_y;
            std::cout<<"Ответ -- "<<makeDecision(makeDecision_x,makeDecision_y);
            break;
        
        case 7:
            int sum3_x,sum3_y,sum3_z;
            std::cout<<"Введитие три числа. Функция выведет true если релуьтат сложения двух из этих чисел будет равен третьему числу \n";
            std::cin>>sum3_x>>sum3_y>>sum3_z;
            std::cout<<"Ответ -- "<<std::boolalpha<<sum3(sum3_x,sum3_y,sum3_z);
            break;
        
        case 8:
            int age_x;
            std::cout<<"Введитие число. Функция выведет коректное написание года для этого числа \n";
            std::cin>>age_x;
            std::cout<<"Ответ -- "<<age(age_x);
            break;
        
        case 9:
        {
            std::string printDays_x;
            std::cout<<"Введитие день недели. Функция выведет все остальные дни до конца недели \n";
            std::cin>>printDays_x;
            std::cout<<"Ответ -- ";
            printDays(printDays_x);
            break;
        }
        case 10:
            int reverseListNums_x;
            std::cout<<"Введитие число. Функция выведет все числа от этого числа до 0 \n";
            std::cin>>reverseListNums_x;
            std::cout<<"Ответ -- "<<reverseListNums(reverseListNums_x);
            break;
        
        case 11:
            int pow_x,pow_y;
            std::cout<<"Введитие два числа. Функция возведет первое число в степень равную второму числу \n";
            std::cin>>pow_x>>pow_y;
            std::cout<<"Ответ -- "<<pow(pow_x,pow_y);
            break;
        
        case 12:
            int equalNum_x;
            std::cout<<"Введитие число. Функция выведет true если все цифры числа одиноковые \n";
            std::cin>>equalNum_x;
            std::cout<<"Ответ -- "<<std::boolalpha<<equalNum(equalNum_x);
            break;
            
        case 13:
        {
            int leftTriangle_x;
            std::cout<<"Введитие число. Функция нарисует треугольник высотой равной числу \n";
            std::cin>>leftTriangle_x;
            leftTriangle(leftTriangle_x);
            break;
        }
        default:
            std::cout<<"Неверная команда";
    }
    return 0;
}
