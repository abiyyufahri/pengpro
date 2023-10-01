# pengpro

Tugas Pengenalan Pemrograman

- Materi 1 - Matematika A
- Materi 1 - Matematika B
- Materi 1 - Matematika 3 Digit

```

package main

import (
	"fmt"
)

func main() {
	var a int

	fmt.Println("-=-= Halo Abiyyu, Ini Golang pertama kamu =-=-")
	fmt.Println(" ")
	fmt.Println("1 : Materi 1 - Matematika A")
	fmt.Println("2 : Materi 1 - Matematika B")
	fmt.Println("3 : Materi 1 - Tiga Digit")
	fmt.Println(" ")
	fmt.Println("Pilih fungsi : ")
	fmt.Scan(&a)

	if a == 1 {
		f1()
	} else if a == 2 {
		f2()
	} else if a == 3 {
		ambil3Karakter()
	} else {
		fmt.Println("Error : pilhan tidak ada")
		fmt.Println("Program End")
	}

	fmt.Println(" ")
	// y := 7
	// y := 7
}

func f1() {
	fmt.Println("-=-= Materi 1 - Matematika A =-=-")
	var x, y int
	fmt.Print("Masukkan nilai x : ")
	fmt.Scan(&x)
	fmt.Print("Masukkan nilai y : ")
	fmt.Scan(&y)
	var z1, z2, z3, zn float64
	z1 = 1
	z2 = float64(3 * (x * x))
	z3 = float64((10 * y) + 7)
	zn = float64(z1/z2 + z3)

	fmt.Println(" ")
	fmt.Println("-=-==========-=-")
	fmt.Print("\nNilai x : ", x)
	fmt.Print("\nNilai y : ", y)
	fmt.Println("\nHasilnya adalah : ", zn)
	fmt.Println("-=-==========-=-")
	fmt.Println(" ")
}

func f2() {
	fmt.Println("-=-= Materi 1 - Matematika B =-=-")
	var x int
	fmt.Print("Masukkan nilai x : ")
	fmt.Scan(&x)
	var z1, z2, zn float64
	z1 = (float64(x * x * x)) + (3 * float64(x))
	z2 = (float64(x * x * x * x)) - (3 * float64(x*x)) + 4
	zn = z1 / z2

	fmt.Println(" ")
	fmt.Println("-=-==========-=-")
	fmt.Print("\nNilai x : ", x)
	fmt.Println("\nHasilnya adalah : ", zn)
	fmt.Println("-=-==========-=-")
	fmt.Println(" ")
}

func ambil3Karakter() {
	fmt.Println("-=-= Materi 1 - Tugas Digit =-=-")

	var input string
	fmt.Print("Masukkan string: ")
	fmt.Scan(&input)

	if len(input) > 3 {
		fmt.Println("String terlalu panjang, harus 3 karakter >:( .")
		return
	}

	fmt.Println(" ")
	fmt.Println("-=-==========-=-")
	if len(input) == 1 {
		x := input[0]
		y := "0"
		z := "0"
		input = input + "00"
		fmt.Printf("x = %s, maka d1 = %c, d2 = %s, dan d3 = %s\n", input, x, y, z)
	} else if len(input) == 2 {
		x := input[0]
		y := input[1]
		z := "0"
		input = input + "0"
		fmt.Printf("x = %s, maka d1 = %c, d2 = %c, dan d3 = %s\n", input, x, y, z)
	} else {
		x := input[0]
		y := input[1]
		z := input[2]
		fmt.Printf("x = %s, maka d1 = %c, d2 = %c, dan d3 = %c\n", input, x, y, z)
	}
	fmt.Println("-=-==========-=-")

}
```

Sekian dari saya Terimakasih.
