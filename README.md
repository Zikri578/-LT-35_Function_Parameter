# -LT-35_Function_Parameter

Function parameter di JavaScript adalah input yang diterima oleh function ketika function tersebut dipanggil. Parameter dapat digunakan dalam function untuk menentukan aksi yang akan dilakukan atau untuk menentukan nilai dari variabel yang digunakan dalam function.

Pada saat mendefinisikan function, parameter didefinisikan di dalam tanda kurung, di mana setiap parameter di pisahkan oleh koma. Contoh: 

    function add(a, b) {
      return a + b;
    }

Pada saat memanggil function, nilai yang sesuai dengan parameter harus diteruskan. Contoh: 

    let result = add(1, 2);

Pada contoh di atas, 1 akan di asign ke parameter `'a'` dan 2 akan di asign ke parameter `'b'` dan function akan mengembalikan hasil dari a + b yaitu 3. Anda juga dapat memberikan parameter default untuk function, yang akan digunakan jika tidak ada nilai yang diteruskan saat function dipanggil.

    function greet(name = 'stranger') {
        console.log("Hello, " + name);
    }
    greet(); // Output: "Hello, stranger"

Secara keseluruhan, parameter dalam function memungkinkan Anda untuk mengirim input ke function dan digunakan dalam operasi yang dilakukan oleh function. Ini membuat function lebih fleksibel dan dapat digunakan dalam berbagai konteks dengan input yang berbeda.

Selain itu, parameter juga dapat digunakan untuk membuat function lebih reusability, dengan mengubah input yang diterima, function dapat digunakan dalam berbagai situasi. 

Selain itu, javascript juga menyediakan fitur untuk menerima parameter yang tidak terbatas jumlahnya atau variadic function dengan menggunakan tanda tiga titik (...) sebelum parameter yang akan menerima parameter yang tidak terbatas. Contoh:

    function sum(...numbers) {
        let result = 0;
        for (let number of numbers) {
            result += number;
        }
        return result;
    }
    console.log(sum(1, 2, 3, 4)); // Output: 10

Pada contoh di atas, function `"sum"` menerima parameter yang tidak terbatas jumlahnya dan menjumlahkan semua parameter yang diterima.

Secara keseluruhan, parameter dalam function memungkinkan Anda untuk menerima input yang berbeda dan menggunakannya dalam operasi yang dilakukan oleh function, membuat function lebih fleksibel dan dapat digunakan dalam berbagai konteks.
