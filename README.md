Q1:
Console.WriteLine("請輸入你的名字");
string name = Console.ReadLine();

Q2:
Console.WriteLine("請輸入數字1或2(1.女生 2.男生)");
string grade = Console.ReadLine();
if(grade!=1 & grade!=2 );
{
 Console.WriteLine("請輸入數字1或2");
 goto Q2;
}

Q3:
Console.WriteLine("請輸入你的出生年月日");
string birth = Console.ReadLine();

Console.WriteLine("請輸入你的學號");
string id = Console.ReadLine();

Console.WriteLine(name);

switch(grade){
    case"1":
        Console.WriteLine("女生");
        break;

    case"2":
        Console.WriteLine("男生");
        break;
}

choose:
Console.WriteLine(birth );
Console.WriteLine(id);
Console.WriteLine("資料正確請按1");
Console.WriteLine("資料有誤請按2");
string check  = Console.ReadLine();
switch(check)
{
    case"1":
    Console.WriteLine("已完成資料建設");
    break;

    case"2":
        Console.WriteLine("請輸入1-4錯誤之資料(1.姓名 2.性別 3.生日 4.學號)");
        string choose =  Console.RriteLine();

        switch(choose)
        {

            case"1":
            goto Q1;
    
            case"2":
            goto Q2;

            case"3":
            goto Q3;

            case"4":
            goto Q4;

            default:
            Console.WriteLine("請輸入1-4錯誤之資料(1.姓名 2.性別 3.生日 4.學號)");
            goto choose;
        }
break;
}
