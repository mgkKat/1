# 1
class DateTime
{
public:
    // конструктор с тремя числовыми параметрами (день, месяц,год);
    DateTime(const int, const int, const int);
    // конструктор без параметров (объект использует текущую дату);
    DateTime();
    // конструктор копирования (создаём копию другого объекта);
    DateTime(const DateTime &) = default;
    // метод main
    int main();
    // для вывода на экран текущей даты в виде строки, с указанием дня недели и названия месяца;
    void printToday() const;
    // для вывода на экран даты вчерашнего дня в виде строки, с указанием дня недели и названия месяца;
    void printYesterday() const;
    // для вывода на экран даты завтрашнего дня в виде строки, с указанием дня недели и названия месяца.
    void printTomorrow() const;
    // для вывода даты через N дней в будущем;
    void printFuture(const int) const;
    // для вывода даты через N дней в прошлом;
    void printPast(const int) const;
    // для вывода названия текущего месяца;
    void printMonth() const;
    // для вывода названия текущего дня недели;
    void printWeekDay() const;
    // для расчёта разницы (в днях) между двумя датами
    int calcDifference(const DateTime &) const;
    
private:
    tm data;
};
