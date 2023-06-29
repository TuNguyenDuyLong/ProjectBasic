# ProjectBasic
ProjectBasic
console.log("Helllo Word")
let name = "Long" // this is a variable
// js is case-sensitive: Có phân biệt hoa thường
let Name = "Jony"
console.log("name:" + name + ", name:" + Name )
/**
 * commet nhiều dòng
 * 
 */
let x = 10
console.log("x:" +x)
// const: gán cho 1 cá thể độc lập
// Ví dụ:
const conguoiyeu = false
console.log(conguoiyeu)
let car = [
    'Mercedes',
    'MC',
    , // empty item
    'Lambor',
    'Fera'
]
console.log(car[1])
let message = "I like these car\
And many other\
Please buy and buy\
"
console.log(message)
// \n\ xuống dòng khi viết văn bản
let  i = 0
while(i<10){
    i=i+1 // nếu để i++ vẫn được
    console.log(`i = ${i}`) // dòng i= thay bằng item vẫn được
}
// Câu lệnh if/else if/else:
let marks = 8.5
if(marks >= 0 && marks <4)
{console.log("Bad")}
else if (marks >=4 && marks < 6)
{console.log("Normal")}
else if (marks >=6 && marks < 8)
{console.log("Good")}
else if (marks >=8 && marks < 10)
{console.log("Excellent")}
else
{console.log("Mark is underfined") }

//Vòng lặp for/ for loot 
for (let i = 0; i <10; i++) {
    if (i %2==0){ // có thể thay đổi điều kiện khác
        continue // có thể dùng câu lệnh break thì se thoát khỏi vòng lặp mà chạy thẳng đến dòng 54
    }
    console.log(`i=${i}`) // nhớ câu lệnh này khi xuất 1 biến trong vòng lặp
}
let cars = [
    'Mercedes',
    'MC',
    'Vin',
    'Toyota',
    'Lambor',
    'Fera'
]
for (let i = 0; i <cars.length -1; i++)
{ console.log(cars[i])}
// Cách 2 sử dụng hàm for each
cars.forEach(function(car){
    console.log(car)
})
// Cách 3 rút gọn từ cách 2:
cars.forEach((car) => {
    console.log(car)
})
// Cách 4: dùng "for of"
for (let dem of cars)
{
    console.log(`name: ${dem}`)
}
//Cách 5: dùng "for in"
for (let dem in cars)
{
    console.log(`name: ${dem}`)
    //console.log("name:" +dem) giống như dòng trên
}
cars.forEach((car, index, array) => {
    console.log(`${index+1}-${car}`)
})
/////////////////
cars.push("EQS Mercedes Sedan")
console.log(cars)
let filteredCars = cars.filter(function(car){
    return car.includes("Mer")
})
console.log(`filteredCars = ${filteredCars}`)
console.log(`Chúng ta tìm thấy được ${filteredCars.length} car`) // Câu lệnh cho biết được số index mà mình tìm (không trả kết quả về tên)
///////////////
let someNumbers = [3, 2, 4, 6, 7, 8]
someNumbers[0] = 5
let AnhXa = someNumbers.map(eachNumbers => {
    return eachNumbers ** 2
})
console.log(`SomeNumbers ${someNumbers}`)
console.log(`AnhXa ${AnhXa}`)
// Xóa tất cả các số nhỏ hơn 5 
// Dùng lệnh after Deleted
console.log("After Deleted")
someNumbers = someNumbers.filter(eachNumbers => eachNumbers >=5)
console.log("someNumbers: " + `${someNumbers}`)
// function:
function sayhello(name)
{
    console.log(`Hello ${name}`)
}
sayhello('Long ')
// function Multiply (x,y)  có thể viết function như thế này
const multiply = function (x,y)
{
    return x*y
}
console.log(`Multiply 5 and 7 = ${multiply(5,7)}`)
