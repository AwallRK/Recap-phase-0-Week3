# Recap-phase-0-Week3


- [Object](#object-literal)
- [Object Array](#object-array)
- [References for Self-Taught](#references-for-self-taught)

![](https://media4.giphy.com/media/wpoLqr5FT1sY0/giphy.gif?cid=ecf05e47hbnc3m5rdrk38ce4wuzg8y6otyy9j5mxr7vyivu1&rid=giphy.gif&ct=g)

# Object Literal

- Setiap object memiliki key/property/attribute yang berbentuk `key:value`
- Nama sebuah key biasanya hanya 1 kata. Namun jika kita ingin membuat key yang terdiri dari 2 kata atau lebih, kita bisa mengggunakan `" "`. Contoh `"angka bagus": 10`.
- object menggunakan {}
- Setiap key pada object bersifat unik.
- Contoh:

```js
// define object
let object = {
  prop1: "Hello",
  prop2: "World",
  "user age": 15,
  prop3: "Lovely Heart"
}

// get key from object

// use . jika kita ingin mengakses langsung key yang terdiri dari 1 kata nya namun tidak bisa digunakan untuk ketika key 2 kata ataupun key berasal dari value variable lain.. contohnya :
console.log(object.prop1)
console.log(object.prop2)


// use [key] jika kita ingin mengakses key dengan 2 suku kata ataupun key yang berasal dari variable contohnya :
//contoh 2 suku kata
console.log(object["user age"])
// contoh jika key berasal dari variable
let key = "prop3"
console.log(object[key])

//how to access every value on object :

for(let key in object){ // loop untuk object dimana didalam terdapat variable key untuk menampung properti tiap objectnya nya.
console.log(key) // akan menampilkan tiap key nya
console.log(object[key]) // akan menampilkan value dari tiap key nya
}

// update value of a key
object.prop1 = "Test"
object['prop3'] = 'angry bird'

//how to delete key on object
delete object['prop3'] // bisa langsung menggunakan delete untuk menghapus objectnya


//how to change array into object 
let arr = ["merah", "biru", "kuning", "hijau", "hijau", "biru", "kuning", "merah"]

//pertama siapkan penampung, karena kita akan menconvert kedalam object kita buat object kosong terlebih dulu
let result = {}

//loop tiap element dalam arr menggunakan loop array
 
for(let i = 0; i < arr.length; i++){

    let perValue = arr[i]
    //karena yang diminta tiap value dalam array ini akan menjadi property, maka lakukan pengecekan property dalam object yang kita buat.

    if(result[perValue] === undefined){ // kondisi ini akan mengecek apakah property pervaluenya ada? jika tidak ada kalian perlu membuatnya

    result[perValue] = 0 // karena yang dicari adalah count dari tiap value maka nilai awal dari tiap property adalah 0
    }
    
    result[perValue]++ // setelah itu ketika propertynya ada dan sama, maka akan di increment valuenya sebanyak 1
}

```

# Object Array

- Array yang terdiri dari kumpulan object

![](https://media3.giphy.com/media/l3q2K5jinAlChoCLS/giphy.gif?cid=ecf05e47sr3vwmvjp1lqn8i27gjowoilvkw2rtbewfojv682&rid=giphy.gif&ct=g)

- Contoh:

```js
let person1 = {
  name: "James"
}
let person2 = {
  name: "Bond"
}
let objects = [person1, person2]

// get key from one of the object in array
objects[0].name // James
```

# References for Self-Taught

![](https://media2.giphy.com/media/3o7abGQa0aRJUurpII/giphy.gif?cid=790b76115496294f1dfb6cb86fa8f73cbc58592664d0284a&rid=giphy.gif&ct=g)

- [Objects](https://www.w3schools.com/js/js_objects.asp)
- [Array of Objects](https://www.freecodecamp.org/news/javascript-array-of-objects-tutorial-how-to-create-update-and-loop-through-objects-using-js-array-methods/)

## Video References

- [An Encounter with JavaScript Objects](https://youtu.be/napDjGFjHR0)
- [Object](https://drive.google.com/drive/folders/1BvYvYJeSwBoNMexPbp7jDCYzRchz0kEp)
