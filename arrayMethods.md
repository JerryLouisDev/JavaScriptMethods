Array Methods
____________________________________________________________________________________________________________________________________
.isArray(): Takes in a value and returns true if the value is an array, else it will return false

**Key Point**
Must add "Array" to your equation

Syntax:
array.isArray(object to be tested)

Example:

function testArr(){
  const arrNum = [1,2,3,4]

  console.log(Array.isArray(arrNum))
}

testArr()

Result:

testArr() => true
____________________________________________________________________________________________________________________________________

.includes(): It is a true and false method that determines if a string contains a character of that string.

**Key Point**
When passing in a string to this method, be aware of cap sensitivity

Syntax:
array.includes(searchValue, start)

Example:

const str = 'HEY HEY HEY, Its YA boi Jey!'
console.log(str.includes('HEY'))

const strOne = 'HEY GOOD MORNING EVERYONE, HEY be GRRRREAT'
console.log(strOne.includes('hey'))

Result:
console.log(str.includes('HEY')) => true
console.log(strOne.includes('hey')) => false
____________________________________________________________________________________________________________________________________

.indexOf() & .lastIndexOf(): searches and indicates an array item and returns its position

Syntax:
array.indexOf(item, start)

Example:

const nbaPlayers = ['Lebron James', 'Kobe Bryant', 'Micheal Jordan', 'James Harden']

console.log(nbaPlayers.indexOf('Micheal Jordan'))

Result:
console.log(nbaPlayers.indexOf('Micheal Jordan')) => 2
____________________________________________________________________________________________________________________________________

.join(): Returns the array as a string

Syntax:
array.join(separator)

Example:

const num = ['1','2','3','4','5']
console.log(num.join(' + '))

Result:
console.log(num.join(' + ')) => 1 + 2 + 3 + 4 + 5
____________________________________________________________________________________________________________________________________

.slice(): This is a method that returns a new array object from the starting argument
and ends at the ending argument but does not include it.

Syntax:
array.slice(start, end)

Example:

const carMake = ['Acura', 'Honda', 'Toyota', 'Tesla', 'Ford', 'Mini Cooper', 'Bentley', 'BMW', 'Kia']
console.log(carMake.slice(2,5))

Result:
console.log(carMake.slice(2,5)) => [ 'Toyota', 'Tesla', 'Ford' ]
____________________________________________________________________________________________________________________________________

.concat(): This method is used to join two or more arrays and returns a new array that contains the joined arrays

Syntax:
array1.concat(array2,...,arrayZ)

Example:

const carMake1 = ['Acura', 'BMW', 'Mercedes-Benz']

const carMake2 = ['Tesla', 'Toyota', 'Bentley']
console.log(carMake1.concat(carMake2))

Result:
console.log(carMake1.concat(carMake2)) => [ 'Acura', 'BMW', 'Mercedes-Benz', 'Tesla', 'Toyota', 'Bentley' ]
____________________________________________________________________________________________________________________________________

.reverse(): This method reverses the order of the elements in the array.

Syntax:
array.reverse()

Example:

const consoles = ['XBOX', 'Playstation', 'Game Cube', 'Wii']

console.log(consoles.reverse())

Result:
console.log(consoles.reverse()) => [ 'Wii', 'Game Cube', 'Playstation', 'XBOX' ]
____________________________________________________________________________________________________________________________________

.sort(): This method sorts the items of an array, it can order them alphabetic or numeric from up to down from down to up.

Syntax:
array.sort()

Example:

const carMake = ['Acura', 'Honda', 'Toyota', 'Tesla', 'Ford', 'Mini Cooper', 'Bentley', 'BMW', 'Kia']

console.log(carMake.sort())

Result:
console.log(carMake.sort()) => ['Acura', 'BMW', 'Bentley', 'Ford', 'Honda', 'Kia', 'Mini Cooper', 'Tesla', 'Toyota']
____________________________________________________________________________________________________________________________________

.splice(): This method adds/removes items to/from an array, then returns the removed item

Syntax:
array.splice(index,howmany, itemA,..., itemZ)

Example:

const acuraModels = ['CL','TL','MDX','RSX']
console.log(acuraModels.splice(2, 0, "NSX", "TLX"))

Result:
console.log(acuraModels.splice(2, 0, "NSX", "TLX")) => CL, TL, NSX, TLX, MDX, RSX
____________________________________________________________________________________________________________________________________

.map(): creates a new array to populate when the results provided function on every element when called

Syntax:
array.map(function(currentValue, index, arr), thisValue)

Example:

const nums = [2,4,8,10]
console.log(nums.map(x => x * 2))

Result:
console.log(nums.map(x => x * 2)) => [4,8,16,20]
____________________________________________________________________________________________________________________________________

.filter(): This method returns an array of elements that pass the tested

Syntax:
array.filter(function(currentValue, index, arr), thisValue)

Example:

const bmwModel = [330, 550, 750, 740]
console.log(bmwModel.filter(x => x <= 600))

Result:
console.log(bmwModel.filter(x => x <= 600)) => [330, 550]
____________________________________________________________________________________________________________________________________

.forEach(): This method calls a function for each element in an array, in order

Syntax:
array.forEach(function(currentValue, index, arr), thisValue)

Example:

const benz = ['C', 'E', 'G', 'S']
benz.forEach(x => console.log(x += '-Class'))

Result:
benz.forEach(x => console.log(x += '-Class')) => C-Class, E-Class, G-Class, S-Class
____________________________________________________________________________________________________________________________________

.reduce(): This method provides a function for each value of the array from left to right reducing the array to a single thisValue

Syntax:
array.reduce(function(total, currentValue, currentIndex, arr), initialValue)

Example:

const nums = [23, 93, 5, 16]
console.log(nums.reduce((acc,val) => acc + val))

Result:
console.log(nums.reduce((acc,val) => acc + val)) => 137
____________________________________________________________________________________________________________________________________

.pop(): This method removes the last element from an array and returns the element

Syntax:
array.pop()

Example:

const toyotaModels = ['Camry', 'MR2', '4Runner', 'Celica', 'Land Cruiser', 'Corolla', 'Highlander']
console.log(toyotaModels.pop())

Result:
console.log(toyotaModels.pop()) => Highlander
____________________________________________________________________________________________________________________________________

.push(): This method adds a new item to the end of an array and returns a new length

Syntax:

Example:


Result:

____________________________________________________________________________________________________________________________________
.shift():

Syntax:

Example:


Result:

____________________________________________________________________________________________________________________________________
