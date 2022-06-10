# playground dosyası
import UIKit
import Darwin

//CLASS EXAMPLE
class Books {
    public var title: String
    private var pageNumber: Int

    init(booksTitle: String, booksPageNumber: Int) {
        self.title = booksTitle
        self.pageNumber = booksPageNumber
    }
    func changeBookTitle(newTitle: String) {
        self.title = newTitle
    }
}


//STRUCT EXAMPLE
struct Movies{
    var name: String
    var min: Float
}
let romantic = Movies(name:"Jeux D'enfants" , min: 1.33)
let action = Movies(name: "Matrix" , min: 2.16 )

print(romantic.name, romantic.min)


//CONTROL FLOW
let writers = ["George Orwell, Tess Gerritsen, Franz Kafka"]
for writer in writers {
    print("My favourite writers \(writer) ")
}

    
    
    //LOOPS
    //FOR
    var total = 0
    for numbers in 0...100 {
        total = total + numbers
    }
    print(total)

    //WHILE
    var month = 1
    while month < 12 {
        print("Today is the \(month) . month of the year")
        month += 1
    }
    print("We are past the 12th month. Happy new year!")

    //SWITCH CASE
    let weatherForecast = 25
    switch weatherForecast{
    case 0...10:
        print("The weather is cold!")
    case 10...20:
        print("The weather is warm")
    case 20...30:
        print("The weather is hot!")
    default:
        print("Unknown")
    }
    
    
    //IF&GUARD
    //IF
    let age = 24

    if age>0 && age<=12 {
        print("You are a child")
        }
    else if age>12 && age<=18 {
        print("You are a teenager")
        }
    else if age>18 && age<=30{
        print("You are a young")
        }
    else if age>30 && age<=50 {
        print("You are an adult")
        }
    else if age>50 {
        print("You are an old")
    }
    else {
        print("You are not born yet")
    }


    //GUARD
    func test(number: Int) -> Bool{
        guard number % 2 == 0 else {
            return false
        }
        return true
    }
    print(test(number: 47))


    //ENUMARATİON
    enum Colors : Int{
        case red = 1,orange,yellow,green,blue,purple,pink,black,white
    }
    let colors = Colors(rawValue: 5)

