# algorithm

- Algorithm C++ standart kütüphanesinde bir container değildir. Tam tersine, algorithm sınıfı, C++ standart kütüphanesinde bulunan bir header dosyasıdır ve STL (Standard Template Library) için kullanılan bir dizi algoritma fonksiyonu sağlar.

- Bu algoritma fonksiyonları, STL'nin temel container sınıfları olan vector, list, set, map gibi sınıflarla birlikte kullanılabilir. algorithm sınıfı, bu container sınıflarının içeriğinde gezinmek ve bu içerikler üzerinde çeşitli işlemler yapmak için kullanılır.

- Örneğin, std::sort, std::find, std::count_if, std::transform gibi algoritma fonksiyonları, bir vector veya list gibi bir container içeriğindeki verileri sıralamak, aramak, saymak veya dönüştürmek için kullanılabilir.



# Fonksiyolar

- **all_of(first, last, pred):** 
> aralıktaki tüm öğelerin pred işlevi tarafından belirtilen özelliğe sahip olup olmadığını kontrol eder. first ve last aralığın başlangıç ve sonunu gösteren işaretçilerdir, pred ise kontrol edilecek özelliği belirten bir işlev nesnesidir.
- **any_of(first, last, pred):** 
> aralıktaki en az bir öğenin pred işlevi tarafından belirtilen özelliğe sahip olup olmadığını kontrol eder.
- **none_of(first, last, pred):** 
> aralıktaki hiçbir öğenin pred işlevi tarafından belirtilen özelliğe sahip olup olmadığını kontrol eder.
- **for_each()** 
> işlevi, bir işlev nesnesi ve bir aralık verildiğinde, aralıktaki her öğe için işlevi çağırır. 
- **for_each_n()**  
> belirli bir sayıda öğe üzerinde bir işlev işlevini uygular. 
- **count()** 
> bir aralıktaki öğelerin belirli bir değere eşit olup olmadığını kontrol etmek için kullanılır. Bu algoritmanın amacı, belirli bir öğe sayısını bulmak istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **count_if()** 
> C++ algoritması, bir aralıktaki öğelerin belirli bir özelliğe sahip olup olmadığını kontrol etmek için kullanılır. Bu algoritmanın amacı, belirli bir özelliğe sahip olan öğe sayısını bulmak istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **mismatch()** 
> iki aralık arasındaki ilk farklı öğeleri bulmak için kullanılır. Bu algoritmanın amacı, iki aralık arasındaki farklılıkları bulmak istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **find()**
> C++ algoritması, bir aralıkta belirli bir öğenin varlığını kontrol etmek için kullanılır. Bu algoritmanın amacı, belirli bir öğenin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **find_if()**
> işlevi, bir aralık ve belirli bir özelliğe sahip olan bir işlev nesnesi verildiğinde, aralıkta öğenin var olup olmadığını kontrol eder.
- **find_if_not()**
> belirli bir özelliğe sahip olmayan öğeleri aramak için kullanılır.
- **find_end()**
> bir aralıkta belirli bir alt aralığın son konumunu bulmak için kullanılır. Bu algoritmanın amacı, belirli bir alt aralığın varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **find_first_of()** 
> bir aralıkta belirli bir öğeler kümesinin ilk konumunu bulmak için kullanılır. Bu algoritmanın amacı, belirli bir öğeler kümesinin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **adjacent_find()**
> bir aralıkta ardışık öğeler arasında bir özellik veya eşleşme aramak için kullanılır. Bu algoritmanın amacı, ardışık öğelerin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **search()**
> bir aralıkta belirli bir alt aralığı aramak için kullanılır. Bu algoritmanın amacı, bir aralıkta alt aralığın varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **search_n()**
> bir aralıkta ardışık bir öğe dizisi aramak için kullanılır. Bu algoritmanın amacı, ardışık öğe dizisinin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

# Modifying sequence operations

- **copy()**
> bir aralıktaki öğeleri başka bir aralığa kopyalamak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri başka bir aralığa taşımak istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **copy_if()**
> bir aralıktaki öğeleri belirli bir koşulu sağlayan öğeleri başka bir aralığa kopyalamak için kullanılır. Bu işlevin kullanımı, std::copy() işlevine benzerdir, ancak kopyalanacak öğeler için bir koşul belirtilir.
- **copy_n()**
> bir aralıktan belirli bir sayıda öğeyi başka bir aralığa kopyalamak için kullanılır. Bu algoritmanın amacı, bir aralıktan belirli bir sayıda öğe kopyalamak istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **copy_backward()**
> bir aralıktaki öğeleri başka bir aralığa sondan başlayarak kopyalamak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri sondan başlayarak başka bir aralığa taşımak istediğinizde kullanımı kolay bir seçenek sunmaktır.
- **move()**
> bir nesneyi taşımak (move) için kullanılır. Bu işlev, bir nesneyi başka bir nesneye atarken, kaynak nesnenin özelliklerinin çalınması (move) için kullanılır. Bu, özellikle büyük nesnelerin kopyalanması için zaman ve bellek kullanımı açısından daha verimli olabilir.
- **move_backward()**
> bir aralıktaki öğeleri sondan başlayarak başka bir aralığa taşımak (move) için kullanılır. Bu işlev, bir nesnenin içeriğini değiştirmeden, sadece nesnenin sahipliğini başka bir nesneye aktarmak için kullanılır. Özellikle büyük veri yapıları ve nesnelerin taşınması için zaman ve bellek kullanımı açısından daha verimlidir.
- **fill()**
>  bir aralığı belirli bir değerle doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir değerle kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.
- **fill_n()**
>  bir aralığı belirli bir değerle belirli bir sayıda doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir değerle kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.
- **transform()**
> bir aralıktaki öğeleri başka bir aralığa dönüştürmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir işlemle değiştirerek başka bir aralığa aktarmak ve bu işlemi hızlı bir şekilde yapmaktır.
- **generate()**
> bir aralığı belirli bir işleme göre doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir işleme göre kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.
- **generate_n()**
> bir aralığı belirli bir işleme göre belirli bir sayıda doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir işleme göre kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.
- **remove()**
> bir aralıktaki öğelerden belirli bir değeri kaldırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir değere göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.
- **remove_if()**
> bir aralıktaki öğelerden belirli bir koşulu sağlayanları kaldırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.
- **remove_copy()**
> bir aralıktan belirli bir öğeyi kaldırarak yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca kopyalamak ve bu işlemi hızlı bir şekilde yapmaktır.
- **remove_copy_if()**
> bir aralıktan belirli bir koşulu sağlayan öğeleri kaldırarak yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca kopyalamak ve bu işlemi hızlı bir şekilde yapmaktır.
- **replace()**
> bir aralıktaki belirli bir değeri başka bir değerle değiştirmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir değere göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.
- **replace_if()**
> bir aralıktaki belirli bir koşulu sağlayan öğeleri başka bir değerle değiştirmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.
- **replace_copy()**
> bir aralıktan belirli bir değeri başka bir değerle değiştirerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir değere göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.
- **replace_copy_if()**
> bir aralıktan belirli bir koşulu sağlayan öğeleri başka bir değerle değiştirerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.
- **swap()**
> iki nesnenin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki nesnenin değerlerini hızlı bir şekilde değiştirmektir
- **swap_ranges()**
> iki aralıktaki öğelerin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki aralıktaki öğelerin değerlerini hızlı bir şekilde değiştirmektir.
- **iter_ranges()**
> iki nesnenin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki nesnenin değerlerini hızlı bir şekilde değiştirmektir.
- **iter_swap()**
> iki nesnenin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki nesnenin değerlerini hızlı bir şekilde değiştirmektir.
- **reverse()**
> bir aralıktaki öğelerin sırasını tersine çevirmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin sırasını hızlı bir şekilde tersine çevirmektir.
- **reverse_copy()**
> bir aralıktaki öğelerin sırasını tersine çevirerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin sırasını hızlı bir şekilde tersine çevirerek yeni bir aralık oluşturmaktır.
- **rotate()**
> bir aralıktaki öğeleri belirli bir konuma kadar döndürmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin belirli bir konuma kadar döndürülmesini sağlamaktır.
- **rotate_copy()**
> bir aralıktaki öğeleri belirli bir konuma kadar döndürerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin belirli bir konuma kadar döndürülmesini sağlayarak yeni bir aralık oluşturmaktır.
- **shift_left()**
> bir aralıktaki öğeleri belirli bir sayıda sol tarafa kaydırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir sayıda sola kaydırarak yeni bir aralık oluşturmaktır.
- **shift_right()**
> bir aralıktaki öğeleri belirli bir sayıda sağ tarafa kaydırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir sayıda sağa kaydırarak yeni bir aralık oluşturmaktır.
- **shuffle()**
> bir aralıktaki öğeleri rastgele bir sıraya yerleştirir. Bu algoritmanın amacı, bir aralıktaki öğelerin rastgele bir sıraya yerleştirilmesidir.
- **sample()**
>  bir aralıktan belirli bir sayıda öğeyi rastgele örneklemek için kullanılır.
- **unique()**
> bir aralıktaki ardışık tekrarlayan öğeleri kaldırır ve ardışık olmayan tekrarlayan öğelerin bir kopyasını yeni bir aralıkta oluşturur.
- **unique_copy()**
> bir aralıktaki ardışık tekrarlayan öğeleri kaldırır ve ardışık olmayan tekrarlayan öğelerin bir kopyasını yeni bir aralıkta oluşturur. std::unique() işlevine benzer, ancak farklı olarak, std::unique_copy() işlevi, kopyalanan benzersiz öğeleri yeni bir aralığa yerleştirir, orijinal aralığı değiştirmez.

# Partitioning operations

- **is_pratitioned()**
>  belirtilen aralıkta öğelerin belirli bir ölçüte göre bölünüp bölünmediğini kontrol eder.
- **partition()**
> bir aralıktaki öğeleri belirli bir ölçüte göre bölerek, ölçüye uyan öğeleri bir tarafa yerleştirir ve uymayanları diğer tarafa yerleştirir. Bu işlev, bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması gerektiğinde sıklıkla kullanılır. Örneğin, bir listedeki çift sayıların tek sayılardan ayrılması gibi durumlarda kullanılabilir.
- **partition_copy()**
> bir aralıktaki öğeleri belirli bir ölçüte göre böler ve iki farklı aralıkta sonuçları saklar. Ölçüye uyan öğeleri birinci aralığa, uymayan öğeleri ikinci aralığa kopyalar. Bu işlev, bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması ve sonuçların ayrı ayrı saklanması gerektiğinde sıklıkla kullanılır.
- **stable_partition()**
> bir aralıktaki öğeleri belirli bir ölçüte göre böler ve ölçüye uyan öğeleri bir tarafa yerleştirir, uymayan öğeleri ise diğer tarafa yerleştirir. Bu işlev, std::partition() işlevi ile aynı işi yapar ancak sırayı korur. Bu nedenle, bu işlev, özellikle sıra önemli olduğunda kullanılır.
- **partition_point()**
> bir aralıktaki öğeleri belirli bir ölçüte göre böldükten sonra, bölme noktasını belirlemek için kullanılır. Bölme noktası, ölçüye uymayan öğelerin başladığı noktadır. Bu işlev, özellikle std::partition() işleviyle birlikte kullanıldığında faydalıdır.

# Sorting Operations

- **is_sorted()**
> bir aralıktaki öğelerin belirli bir sıraya göre sıralanıp sıralanmadığını kontrol eder. 
- **is_sorted_until()**
> bir aralıktaki öğelerin belirli bir sıraya göre sıralanmış olduğu son öğenin işaretçisini döndürür. Bu işlev, std::is_sorted() işlevine benzerdir ancak sıralı olan öğelerin sonuncusunu işaret eder.
- **sort()**
> bir aralıktaki öğeleri belirli bir sıraya göre sıralar. Bu işlev, C++'ın standart kitaplığındaki en önemli ve en sık kullanılan işlevlerden biridir.
- **partial_sort()**
> bir aralıktaki öğelerin bir kısmını belirli bir sıraya göre sıralar. Bu işlev, genellikle öncelikli olarak ilk N öğeyi sıralamak istediğiniz durumlarda kullanılır.
- **partial_sort_copy()**
>  bir aralıktaki öğelerin bir kısmını belirli bir sıraya göre sıralar ve sıralanmış öğeleri başka bir aralığa kopyalar. Bu işlev, std::partial_sort() işlevine benzer, ancak sıralanmış öğeleri yeni bir aralığa kopyalar.
- **stable_sort()**
> bir aralıktaki öğeleri belirli bir sıraya göre sıralar. Bu işlev, std::sort() işlevine benzer, ancak sıralama işlemi sırasında öğelerin orijinal sıralama ilişkisi korunur. Bu nedenle, std::stable_sort() işlevi, öğelerin birbirine göre ilişkisini korumak istediğiniz durumlarda kullanılabilir.
- **nth_element()**
> bir aralıktaki öğelerin sadece belirli bir sıralamada olan n'inci öğesini bulmak için kullanılır. Bu işlev, özellikle büyük aralıkların sıralanması gerektiğinde ve sadece birkaç öğenin sıralanması gerektiğinde faydalıdır.

# Binary Search Operations (On Sorted Ranges)
- **lower_bound()**
> bir aralıkta belirli bir değere veya daha büyük ilk değere sahip olan ilk öğenin konumunu (iterator'ünü) döndürür. Bu işlev, özellikle sıralanmış bir aralıkta bir değerin veya belirli bir değerden büyük ilk öğenin konumunu bulmak için kullanılır.
- **upper_bound()**
> bir aralıkta belirli bir değerden büyük ilk öğenin konumunu (iterator'ünü) döndürür. Bu işlev, özellikle sıralanmış bir aralıkta bir değerden büyük ilk öğenin konumunu bulmak için kullanılır.
- **binary_search()**
> sıralı bir aralıkta belirli bir değerin olup olmadığını kontrol eder. Eğer aralıkta değer varsa, true değerini döndürür; yoksa false değerini döndürür.
- equal_range()

# Other Operations on Sorted Ranges
- merge
- inplace_merge

# Set Operations (On Sorted Ranges)
- includes()
- set_difference()
- set_intersections()
- set_symmetric_difference()
- set_union()

# Heap Operations
- is_heap()
- is_heap_until()
- make_heap()
- push_heap()
- pop_heap()
- sort_heap()

# Minimum/ Maximum Operations
- max()
- max_element()
- min()
- min_element()
- minmax()
- minmax_element()
- clamp()

# Comparison Operations
- equal
- lexicographical_compare
- lexicographical_compare_three_way

# Permutation Operations
- is_permuatation
- next_permutation
- prev_permutation

# IMPLEMENTATIONS

## Fonksiyolar 

### all_of - any_of - none_of

- Bu üç C++ algoritması, bir aralıktaki öğelerin belirli bir özelliğe sahip olup olmadığını kontrol etmek için kullanılır. İşlevlerin sözdizimi şu şekildedir:

- **std::all_of(first, last, pred):** aralıktaki tüm öğelerin pred işlevi tarafından belirtilen özelliğe sahip olup olmadığını kontrol eder. first ve last aralığın başlangıç ve sonunu gösteren işaretçilerdir, pred ise kontrol edilecek özelliği belirten bir işlev nesnesidir.
- **std::any_of(first, last, pred):** aralıktaki en az bir öğenin pred işlevi tarafından belirtilen özelliğe sahip olup olmadığını kontrol eder.
- **std::none_of(first, last, pred):** aralıktaki hiçbir öğenin pred işlevi tarafından belirtilen özelliğe sahip olup olmadığını kontrol eder.

- Bu işlevler C++11'de tanıtılmıştır ve C++17'de C++ aralık ifadeleri (std::ranges) için de tanıtılmıştır.

- İşte bir örnek kod parçası, bu işlevlerin nasıl kullanıldığını gösteriyor: 

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5};

  if (std::all_of(my_vec.begin(), my_vec.end(), [](int i){return i > 0;})) {
    std::cout << "Tüm öğeler pozitif" << std::endl;
  } else {
    std::cout << "Tüm öğeler pozitif değil" << std::endl;
  }

  if (std::any_of(my_vec.begin(), my_vec.end(), [](int i){return i % 2 == 0;})) {
    std::cout << "En az bir öğe çift" << std::endl;
  } else {
    std::cout << "Hiçbir öğe çift değil" << std::endl;
  }

  if (std::none_of(my_vec.begin(), my_vec.end(), [](int i){return i < 0;})) {
    std::cout << "Hiçbir öğe negatif değil" << std::endl;
  } else {
    std::cout << "En az bir öğe negatif" << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::all_of(), std::any_of() ve std::none_of() işlevlerinin kullanımını göstermektedir. std::vectorint türünde bir vektör oluşturuyoruz ve bu vektörün öğelerinin pozitif, çift veya negatif olup olmadığını kontrol ediyoruz.

> Her işlev, belirtilen özelliğe sahip olan öğe sayısına göre true veya false değeri döndürür. Yukarıdaki kodda, std::all_of() işlevinin sonucu true olarak döndürür çünkü tüm öğeler pozitiftir. std::any_of() işlevi, en az bir çift sayı içeren vektörde true döndürürken, std::none_of() işlevi, herhangi bir negatif öğe içermeyen bir vektörde true döndürür.

Bu işlevlerin kullanımı, bir aralıktaki öğelerin özelliklerini kontrol etmek için oldukça yaygındır ve STL algoritmalarının güçlü bir parçasıdır.

### for_each

- std::for_each() C++ algoritması, bir aralıktaki öğeler üzerinde bir işlev işlevini uygular. Bu algoritmanın amacı, bir dizi işlemi bir aralık üzerinde uygulamak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::for_each() işlevi, bir işlev nesnesi ve bir aralık verildiğinde, aralıktaki her öğe için işlevi çağırır. İşlev nesnesi, aralıktaki her öğe için çağrılacak işlevi belirtir. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt, class UnaryFunction>
UnaryFunction for_each(InputIt first, InputIt last, UnaryFunction f);

```
- Bu işlevin ilk iki parametresi, aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son parametre, aralıktaki her öğe için çağrılacak işlevi belirten bir işlev nesnesidir. İşlev, aralıktaki her öğe için çağrıldığında işlevin geri dönüş değeri kullanılmaz.

- İşte bir örnek kod parçası, std::for_each() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

void print_num(int num) {
  std::cout << num << " ";
}

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5};

  std::for_each(my_vec.begin(), my_vec.end(), print_num);

  return 0;
}

```
> Bu örnek kod, std::for_each() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektördeki her öğeyi ekrana yazdırmak için print_num() işlevini kullanıyoruz. std::for_each() işlevi, print_num() işlevini her öğe için çağırır ve sonuç olarak 1 2 3 4 5 değerlerini ekrana yazdırır.

- Bu işlevin kullanımı, bir aralıktaki öğeleri bir dizi işlem için kullanmak istediğiniz durumlarda oldukça yaygındır. Örneğin, bir vektördeki tüm öğeleri toplamak veya bir dosyadaki tüm satırları okumak için kullanılabilir.

### for_each_n 

- std::for_each_n() C++ algoritması, belirli bir sayıda öğe üzerinde bir işlev işlevini uygular. 
- std::for_each_n() işlevi, std::for_each() işlevine benzer şekilde çalışır, ancak işlemin uygulanacağı öğe sayısı belirtilir. Bu, özellikle büyük aralıklarda sadece belirli bir sayıda öğe üzerinde işlem yapmak istediğinizde faydalıdır.

- std::for_each_n() işlevi, bir işlev nesnesi ve bir başlangıç konumu ve işlemin uygulanacak öğe sayısı verildiğinde, belirtilen sayıdaki öğeler için işlevi çağırır. İşlev nesnesi, her öğe için çağrılacak işlevi belirtir. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt, class Size, class UnaryFunction>
InputIt for_each_n(InputIt first, Size count, UnaryFunction f);

```

- Bu işlevin ilk parametresi, işlem başlangıç noktasını gösteren bir işaretçidir. İkinci parametre, işlem yapılacak öğe sayısını belirtir. Son parametre, aralıktaki her öğe için çağrılacak işlevi belirten bir işlev nesnesidir. İşlev, belirtilen sayıdaki öğeler için çağrılır ve son öğenin ardından işaretçi döndürülür.

- İşte bir örnek kod parçası, std::for_each_n() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

void print_num(int num) {
  std::cout << num << " ";
}

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5};

  std::for_each_n(my_vec.begin(), 3, print_num);

  return 0;
}

```
> Bu örnek kod, std::for_each_n() işlevinin kullanımını göstermektedir. std::vectorint türünde bir vektör oluşturuyoruz ve ilk üç öğeyi ekrana yazdırmak için print_num() işlevini kullanıyoruz. std::for_each_n() işlevi, print_num() işlevini ilk üç öğe için çağırır ve sonuç olarak 1 2 3 değerlerini ekrana yazdırır.

- Bu işlevin kullanımı, bir aralıktaki öğelerin belirli bir sayıda öğesine işlem yapmak istediğiniz durumlarda oldukça yaygındır. Örneğin, bir dosyadaki ilk 10 satırı okumak için kullanılabilir.

### count

- std::count() C++ algoritması, bir aralıktaki öğelerin belirli bir değere eşit olup olmadığını kontrol etmek için kullanılır. Bu algoritmanın amacı, belirli bir öğe sayısını bulmak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::count() işlevi, bir aralık ve belirli bir değer verildiğinde, aralıktaki öğelerin kaçının belirtilen değere eşit olduğunu sayar. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt, class T>
typename iterator_traits<InputIt>::difference_type count(InputIt first, InputIt last, const T& value);

```

- Bu işlevin ilk iki parametresi, aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son parametre, sayılacak öğelerin değeridir. İşlev, aralıktaki öğelerin kaçının belirtilen değere eşit olduğunu sayar ve sonuç olarak belirtilen değere eşit olan öğe sayısını döndürür.

- İşte bir örnek kod parçası, std::count() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 2, 3, 2, 4, 2, 5};

  int count = std::count(my_vec.begin(), my_vec.end(), 2);

  std::cout << "Vektördeki 2 sayısı " << count << " kez geçiyor" << std::endl;

  return 0;
}

```

> Bu örnek kod, std::count() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektördeki 2 sayısının kaç kez geçtiğini saymak için std::count() işlevini kullanıyoruz. std::count() işlevi, vektördeki 2 sayısının 4 kez geçtiğini sayar ve sonuç olarak 4 değerini döndürür.

- Bu işlevin kullanımı, bir aralıktaki öğelerin belirli bir değere eşit olup olmadığını kontrol etmek için oldukça yaygındır. Örneğin, bir kelime içinde belirli bir karakterin kaç kez geçtiğini saymak veya bir dosyadaki belirli bir kelime sayısını saymak için kullanılabilir.

### count_if

- std::count_if() C++ algoritması, bir aralıktaki öğelerin belirli bir özelliğe sahip olup olmadığını kontrol etmek için kullanılır. Bu algoritmanın amacı, belirli bir özelliğe sahip olan öğe sayısını bulmak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::count_if() işlevi, bir aralık ve belirli bir özelliği kontrol eden bir işlev verildiğinde, aralıktaki öğelerin kaçının belirtilen özelliğe sahip olduğunu sayar. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt, class UnaryPredicate>
typename iterator_traits<InputIt>::difference_type count_if(InputIt first, InputIt last, UnaryPredicate p);

```

- Bu işlevin ilk iki parametresi, aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son parametre, her öğe için çağrılacak bir işlev nesnesidir ve belirli bir özelliği kontrol eder. İşlev, aralıktaki öğelerin kaçının belirtilen özelliğe sahip olduğunu sayar ve sonuç olarak belirtilen özelliğe sahip olan öğe sayısını döndürür.

- İşte bir örnek kod parçası, std::count_if() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int num) {
  return num % 2 == 0;
}

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5};

  int count = std::count_if(my_vec.begin(), my_vec.end(), is_even);

  std::cout << "Vektördeki çift sayıların sayısı: " << count << std::endl;

  return 0;
}

```

> Bu örnek kod, std::count_if() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektördeki çift sayıların sayısını saymak için is_even() işlevini kullanıyoruz. std::count_if() işlevi, vektördeki çift sayıların sayısını sayar ve sonuç olarak 2 değerini döndürür.

- Bu işlevin kullanımı, bir aralıktaki öğelerin belirli bir özelliğe sahip olup olmadığını kontrol etmek için oldukça yaygındır. Örneğin, bir dosyadaki belirli bir kelimeyi içeren satırların sayısını saymak veya bir dosyadaki belirli bir karakterin sayısını saymak için kullanılabilir.

### mismatch

- std::mismatch() C++ algoritması, iki aralık arasındaki ilk farklı öğeleri bulmak için kullanılır. Bu algoritmanın amacı, iki aralık arasındaki farklılıkları bulmak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::mismatch() işlevi, iki aralık verildiğinde, aralıkların ilk farklı öğesinin konumunu döndürür. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt1, class InputIt2>
std::pair<InputIt1, InputIt2> mismatch(InputIt1 first1, InputIt1 last1, InputIt2 first2);

```
> Bu işlevin ilk iki parametresi, karşılaştırılan ilk aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son parametre, karşılaştırılan ikinci aralığın başlangıç konumunu gösteren bir işaretçidir. İşlev, iki aralık arasında ilk farklı öğeyi bulduğunda, bir std::pair nesnesi döndürür ve bu nesnenin first elemanı ilk aralıktaki farklı öğenin konumunu, second elemanı ise ikinci aralıktaki farklı öğenin konumunu gösterir.

- İşte bir örnek kod parçası, std::mismatch() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec1 {1, 2, 3, 4, 5};
  std::vector<int> my_vec2 {1, 2, 3, 5, 4};

  auto mismatch_pair = std::mismatch(my_vec1.begin(), my_vec1.end(), my_vec2.begin());

  if (mismatch_pair.first != my_vec1.end()) {
    std::cout << "İlk farklı öğe: " << *mismatch_pair.first << " ve " << *mismatch_pair.second << std::endl;
  } else {
    std::cout << "Aralıklar eşleşiyor" << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::mismatch() işlevinin kullanımını göstermektedir. İki std::vector  int türünde vektör oluşturuyoruz ve std::mismatch() işlevini kullanarak iki vektör arasındaki ilk farklı öğeyi buluyoruz. İlk vektördeki 5 ve ikinci vektördeki 4 öğeleri farklı olduğu için std::mismatch() işlevi bir std::pair nesnesi döndürür ve bu nesnenin first elemanı 5'in konumunu, second elemanı ise 4'ün konumunu gösterir.

- Bu işlevin kullanımı, iki aralık arasındaki farklılıkları kontrol etmek için oldukça yaygındır. Örneğin, iki dosya arasındaki farklılıkları bulmak veya iki veritabanı arasındaki farklılıkları kontrol etmek için kullanılabilir.

### find - find_if - find_if_not

- std::find() C++ algoritması, bir aralıkta belirli bir öğenin varlığını kontrol etmek için kullanılır. Bu algoritmanın amacı, belirli bir öğenin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::find() işlevi, bir aralık ve aranacak öğenin değeri verildiğinde, aralıkta öğenin var olup olmadığını kontrol eder. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt, class T>
InputIt find(InputIt first, InputIt last, const T& value);

```
- Bu işlevin ilk iki parametresi, aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son parametre, aranacak öğenin değeridir. İşlev, aralıktaki öğeleri arar ve öğe bulunduğunda öğenin konumunu gösteren bir işaretçi döndürür. Öğe bulunamadığında ise son öğeyi gösteren bir işaretçi döndürülür.

- std::find_if() ve std::find_if_not() işlevleri, belirli bir özelliğe sahip olan veya sahip olmayan öğeleri aramak için kullanılır. std::find_if() işlevi, bir aralık ve belirli bir özelliğe sahip olan bir işlev nesnesi verildiğinde, aralıkta öğenin var olup olmadığını kontrol eder. std::find_if_not() işlevi ise, belirli bir özelliğe sahip olmayan öğeleri aramak için kullanılır.

- İşte örnek bir kod parçası, std::find() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5};

  auto it = std::find(my_vec.begin(), my_vec.end(), 3);

  if (it != my_vec.end()) {
    std::cout << "Öğe bulundu: " << *it << std::endl;
  } else {
    std::cout << "Öğe bulunamadı" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::find() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektörde 3 sayısının olup olmadığını kontrol etmek için std::find() işlevini kullanıyoruz. std::find() işlevi, vektörde 3 sayısının var olduğunu tespit eder ve sonuç olarak 3 sayısının konumunu gösteren bir işaretçi döndürür.

- std::find_if() ve std::find_if_not() işlevlerinin kullanımı da benzerdir. İşlevin ilk iki parametresi aralık işaretçilerdir ve son parametre, bir işlev nesnesidir. İşlev nesnesi, belirli bir özelliğe sahip olan veya sahip olmayan öğeleri tanımlar. İşlev, aralıktaki öğeleri arar ve öğe bulunduğunda öğenin konumunu gösteren bir işaretçi döndürür. Öğe bulunamadığında ise son öğeyi gösteren bir işaretçi döndürülür.

- İşte örnek bir kod parçası, std::find_if() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int num) {
  return num % 2 == 0;
}

int main() {
  std::vector<int> my_vec {1, 3, 5, 7, 8};

  auto it = std::find_if(my_vec.begin(), my_vec.end(), is_even);

  if (it != my_vec.end()) {
    std::cout << "İlk çift sayı: " << *it << std::endl;
  } else {
    std::cout << "Çift sayı bulunamadı" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::find_if() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektördeki ilk çift sayıyı bulmak için is_even() işlevini kullanıyoruz. std::find_if() işlevi, vektördeki ilk çift sayıyı tespit eder ve sonuç olarak çift sayının konumunu gösteren bir işaretçi döndürür.

- std::find_if_not() işlevinin kullanımı da benzerdir, ancak belirli bir özelliğe sahip olmayan öğeleri aramak için kullanılır.

- Bu işlevlerin kullanımı, bir aralıkta belirli bir öğenin varlığını veya belirli bir özelliğe sahip olan veya sahip olmayan öğeleri bulmak için oldukça yaygındır. Örneğin, bir kelime içinde belirli bir karakterin var olup olmadığını kontrol etmek veya bir dosyada belirli bir kelimeyi içeren satırı bulmak için kullanılabilir.

### find_end

- std::find_end() C++ algoritması, bir aralıkta belirli bir alt aralığın son konumunu bulmak için kullanılır. Bu algoritmanın amacı, belirli bir alt aralığın varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::find_end() işlevi, birinci aralık ve ikinci alt aralık verildiğinde, ikinci alt aralığın son konumunu bulur. İşlevin sözdizimi şu şekildedir:

```CPP
template <class ForwardIt1, class ForwardIt2>
ForwardIt1 find_end(ForwardIt1 first1, ForwardIt1 last1, ForwardIt2 first2, ForwardIt2 last2);

```

- Bu işlevin ilk iki parametresi, aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son iki parametre ise alt aralığın başlangıç ve sonunu gösteren işaretçilerdir. İşlev, ilk aralıkta ikinci alt aralığın son konumunu bulduğunda, öğenin konumunu gösteren bir işaretçi döndürür. Alt aralık bulunamadığında ise son öğeyi gösteren bir işaretçi döndürülür.

- İşte örnek bir kod parçası, std::find_end() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5, 1, 2, 3};

  std::vector<int> sub_vec {1, 2, 3};

  auto it = std::find_end(my_vec.begin(), my_vec.end(), sub_vec.begin(), sub_vec.end());

  if (it != my_vec.end()) {
    std::cout << "Alt aralık son konumu: " << std::distance(my_vec.begin(), it) << std::endl;
  } else {
    std::cout << "Alt aralık bulunamadı" << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::find_end() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektördeki alt aralığın son konumunu bulmak için std::find_end() işlevini kullanıyoruz. İkinci vektör, alt aralığı temsil eder. std::find_end() işlevi, vektördeki alt aralığın son konumunu tespit eder ve sonuç olarak alt aralığın son konumunu gösteren bir işaretçi döndürür.

- Bu işlevin kullanımı, bir aralıkta belirli bir alt aralığın son konumunu bulmak için oldukça yaygındır. Örneğin, bir dosyadaki belirli bir kelimeyi içeren son satırın konumunu bulmak veya bir veritabanındaki belirli bir kaydın son konumunu bulmak için kullanılabilir.

### find_first_of

- std::find_first_of() C++ algoritması, bir aralıkta belirli bir öğeler kümesinin ilk konumunu bulmak için kullanılır. Bu algoritmanın amacı, belirli bir öğeler kümesinin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::find_first_of() işlevi, birinci aralık ve ikinci öğeler kümesi verildiğinde, ikinci öğeler kümesindeki herhangi bir öğenin ilk konumunu bulur. İşlevin sözdizimi şu şekildedir:

```CPP
template <class InputIt, class ForwardIt>
InputIt find_first_of(InputIt first1, InputIt last1, ForwardIt first2, ForwardIt last2);

```
- Bu işlevin ilk iki parametresi, aralığın başlangıç ve sonunu gösteren işaretçilerdir. Son iki parametre, öğeler kümesinin başlangıç ve sonunu gösteren işaretçilerdir. İşlev, ilk aralıkta ikinci öğeler kümesindeki herhangi bir öğenin ilk konumunu bulduğunda, öğenin konumunu gösteren bir işaretçi döndürür. Öğeler kümesindeki öğeler aranırken, her bir öğe için arama işlemi aralıktaki öğelerin sırasıyla taranmasıyla gerçekleştirilir. Eğer hiçbir öğe bulunamazsa son öğeyi gösteren bir işaretçi döndürülür.

- İşte örnek bir kod parçası, std::find_first_of() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5};

  std::vector<int> search_vec {4, 5, 6};

  auto it = std::find_first_of(my_vec.begin(), my_vec.end(), search_vec.begin(), search_vec.end());

  if (it != my_vec.end()) {
    std::cout << "İlk eşleşen öğe: " << *it << std::endl;
  } else {
    std::cout << "Eşleşen öğe bulunamadı" << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::find_first_of() işlevinin kullanımını göstermektedir. std::vector int  türünde bir vektör oluşturuyoruz ve vektördeki belirli bir öğeler kümesinin ilk konumunu bulmak için std::find_first_of() işlevini kullanıyoruz. İkinci vektör, öğeler kümesini temsil eder. std::find_first_of() işlevi, vektördeki öğeler kümesindeki ilk eşleşen öğeyi tespit eder ve sonuç olarak öğenin konumunu gösteren bir işaretçi döndürür.

- Bu işlevin kullanımı, bir aralıkta belirli bir öğeler kümesinin varlığını kontrol etmek veya belirli bir öğeler kümesindeki herhangi bir öğenin konumunu bulmak için oldukça yaygındır. Örneğin, bir kelime içinde belirli bir karakter kümesinin ilk konumunu bulmak veya bir veritabanında belirli bir kayıttaki belirli bir alanın değeriyle eşleşen herhangi bir kaydın konumunu bulmak için kullanılabilir.

### adjacent_find

- std::adjacent_find() C++ algoritması, bir aralıkta ardışık öğeler arasında bir özellik veya eşleşme aramak için kullanılır. Bu algoritmanın amacı, ardışık öğelerin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::adjacent_find() işlevi, birinci ve ikinci parametre olarak aralığın başlangıç ve sonunu gösteren işaretçileri alır. İşlev, ardışık öğeler arasında belirli bir özellik veya eşleşme bulduğunda, öğelerin konumunu gösteren bir işaretçi döndürür. Eşleşme bulunamazsa son öğeyi gösteren bir işaretçi döndürülür.

- İşte örnek bir kod parçası, std::adjacent_find() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_consecutive(int x, int y) {
  return y - x == 1;
}

int main() {
  std::vector<int> my_vec {1, 2, 3, 5, 6, 7, 9};

  auto it = std::adjacent_find(my_vec.begin(), my_vec.end(), is_consecutive);

  if (it != my_vec.end()) {
    std::cout << "Ardışık öğelerin ilk konumu: " << std::distance(my_vec.begin(), it) << std::endl;
  } else {
    std::cout << "Ardışık öğeler bulunamadı" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::adjacent_find() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektördeki ardışık öğelerin ilk konumunu bulmak için std::adjacent_find() işlevini kullanıyoruz. İşlev, vektörde ardışık olan 1 ve 2 öğelerini tespit eder ve sonuç olarak öğelerin konumunu gösteren bir işaretçi döndürür.

- Bu işlevin kullanımı, bir aralıkta ardışık öğelerin varlığını kontrol etmek için oldukça yaygındır. Örneğin, bir kelime içinde belirli bir karakter dizisi aramak veya bir veritabanındaki ardışık kayıtları bulmak için kullanılabilir.

### search()
- std::search() C++ algoritması, bir aralıkta belirli bir alt aralığı aramak için kullanılır. Bu algoritmanın amacı, bir aralıkta alt aralığın varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::search() işlevi, birinci ve ikinci parametre olarak aralığın başlangıç ve sonunu gösteren işaretçileri alır. Üçüncü ve dördüncü parametreler, alt aralığın başlangıç ve sonunu gösteren işaretçilerdir. İşlev, alt aralığın ilk konumunu bulduğunda, öğenin konumunu gösteren bir işaretçi döndürür. Alt aralık bulunamazsa son öğeyi gösteren bir işaretçi döndürülür.

- İşte örnek bir kod parçası, std::search() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 3, 4, 5, 1, 2, 3};

  std::vector<int> sub_vec {1, 2, 3};

  auto it = std::search(my_vec.begin(), my_vec.end(), sub_vec.begin(), sub_vec.end());

  if (it != my_vec.end()) {
    std::cout << "Alt aralık ilk konumu: " << std::distance(my_vec.begin(), it) << std::endl;
  } else {
    std::cout << "Alt aralık bulunamadı" << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::search() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektörde belirli bir alt aralığı aramak için std::search() işlevini kullanıyoruz. İkinci vektör, alt aralığı temsil eder. std::search() işlevi, vektördeki alt aralığın ilk konumunu tespit eder ve sonuç olarak alt aralığın ilk konumunu gösteren bir işaretçi döndürür.

- Bu işlevin kullanımı, bir aralıkta belirli bir alt aralığın varlığını kontrol etmek veya belirli bir alt aralığı bulmak için oldukça yaygındır. Örneğin, bir dosyada belirli bir kelimeyi içeren satırı bulmak veya bir veritabanında belirli bir kaydı bulmak için kullanılabilir.

### search_n

- std::search_n() C++ algoritması, bir aralıkta ardışık bir öğe dizisi aramak için kullanılır. Bu algoritmanın amacı, ardışık öğe dizisinin varlığını kontrol etmek istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::search_n() işlevi, birinci ve ikinci parametre olarak aralığın başlangıcını ve sonunu gösteren işaretçileri alır. Üçüncü parametre, ardışık öğe dizisi için gereken öğe sayısıdır. Dördüncü parametre, aranacak öğe değeridir. İşlev, ardışık öğe dizisini bulduğunda, öğelerin konumunu gösteren bir işaretçi döndürür. Ardışık öğe dizisi bulunamazsa son öğeyi gösteren bir işaretçi döndürülür.

- İşte örnek bir kod parçası, std::search_n() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> my_vec {1, 2, 3, 1, 2, 3, 4, 5};

  int count = 2;
  int value = 3;

  auto it = std::search_n(my_vec.begin(), my_vec.end(), count, value);

  if (it != my_vec.end()) {
    std::cout << "Ardışık " << count << " öğe bulundu, ilk konum: " << std::distance(my_vec.begin(), it) << std::endl;
  } else {
    std::cout << "Ardışık öğeler bulunamadı" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::search_n() işlevinin kullanımını göstermektedir. std::vector int türünde bir vektör oluşturuyoruz ve vektörde ardışık bir öğe dizisini bulmak için std::search_n() işlevini kullanıyoruz. count değişkeni, aranacak öğe sayısını ve value değişkeni, aranacak öğe değerini temsil eder. std::search_n() işlevi, vektörde ardışık olan 3 öğelerinin ilk konumunu tespit eder ve sonuç olarak öğelerin konumunu gösteren bir işaretçi döndürür.

- Bu işlevin kullanımı, bir aralıkta ardışık öğelerin varlığını kontrol etmek için oldukça yaygındır. Örneğin, bir dosyada belirli bir karakter dizisi aramak veya bir veritabanında ardışık kayıtları bulmak için kullanılabilir.

### copy

- std::copy() C++ algoritması, bir aralıktaki öğeleri başka bir aralığa kopyalamak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri başka bir aralığa taşımak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::copy() işlevi, birinci ve ikinci parametre olarak kopyalanacak aralığın başlangıcını ve sonunu gösteren işaretçileri alır. Üçüncü parametre, kopyalanacak aralığın başlangıcını gösteren işaretçidir. İşlev, kopyalama işlemini gerçekleştirdikten sonra son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> src {1, 2, 3, 4, 5};
  std::vector<int> dest(5);

  std::copy(src.begin(), src.end(), dest.begin());

  for (auto it = dest.begin(); it != dest.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde src ve dest isimli iki vektör oluşturuyoruz. Ardından, std::copy() işlevini kullanarak src vektöründeki öğeleri dest vektörüne kopyalıyoruz. Son olarak, dest vektöründeki öğeleri yazdırıyoruz.

### copy_if()

- std::copy_if() işlevi, bir aralıktaki öğeleri belirli bir koşulu sağlayan öğeleri başka bir aralığa kopyalamak için kullanılır. Bu işlevin kullanımı, std::copy() işlevine benzerdir, ancak kopyalanacak öğeler için bir koşul belirtilir.

std::copy_if() işlevi, birinci ve ikinci parametre olarak kopyalanacak aralığın başlangıcını ve sonunu gösteren işaretçileri alır. Üçüncü parametre, kopyalanacak aralığın başlangıcını gösteren işaretçidir. Dördüncü parametre, kopyalama koşulunu sağlayan bir işlev veya lambda işlevi olabilir. İşlev, kopyalama işlemini gerçekleştirdikten sonra son konumu gösteren bir işaretçi döndürür.

İşte örnek bir kod parçası, std::copy_if() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int x) {
  return x % 2 == 0;
}

int main() {
  std::vector<int> src {1, 2, 3, 4, 5};
  std::vector<int> dest;

  std::copy_if(src.begin(), src.end(), std::back_inserter(dest), is_even);

  for (auto it = dest.begin(); it != dest.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::copy_if() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde src ve dest isimli iki vektör oluşturuyoruz. Ardından, std::copy_if() işlevini kullanarak src vektöründeki çift sayıları dest vektörüne kopyalıyoruz. Son olarak, dest vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğeleri belirli bir koşulu sağlayan öğeleri seçmek için oldukça yaygındır. Örneğin, bir veritabanından belirli bir koşulu sağlayan kayıtları seçmek için kullanılabilir.

### copy_n

- std::copy_n() C++ algoritması, bir aralıktan belirli bir sayıda öğeyi başka bir aralığa kopyalamak için kullanılır. Bu algoritmanın amacı, bir aralıktan belirli bir sayıda öğe kopyalamak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::copy_n() işlevi, birinci parametre olarak kopyalanacak aralığın başlangıcını gösteren bir işaretçi alır. İkinci parametre, kopyalanacak öğe sayısını belirten bir tamsayıdır. Üçüncü parametre, kopyalanacak öğelerin başlangıcını gösteren işaretçidir. Dördüncü parametre, kopyalama işleminin yapılacağı hedefin başlangıcını gösteren işaretçidir. İşlev, kopyalama işlemini gerçekleştirdikten sonra son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::copy_n() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> src {1, 2, 3, 4, 5};
  std::vector<int> dest(3);

  std::copy_n(src.begin(), 3, dest.begin());

  for (auto it = dest.begin(); it != dest.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::copy_n() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde src ve dest isimli iki vektör oluşturuyoruz. Ardından, std::copy_n() işlevini kullanarak src vektöründen ilk üç öğeyi dest vektörüne kopyalıyoruz. Son olarak, dest vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktan belirli bir sayıda öğe kopyalamak için oldukça yaygındır. Örneğin, bir dosyadan belirli bir sayıda karakter kopyalamak veya bir veritabanından belirli bir sayıda kayıt kopyalamak için kullanılabilir.

### copy_backward

- std::copy_backward() C++ algoritması, bir aralıktaki öğeleri başka bir aralığa sondan başlayarak kopyalamak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri sondan başlayarak başka bir aralığa taşımak istediğinizde kullanımı kolay bir seçenek sunmaktır.

- std::copy_backward() işlevi, birinci ve ikinci parametre olarak kopyalanacak aralığın başlangıcını ve sonunu gösteren işaretçileri alır. Üçüncü parametre, kopyalanacak aralığın sonunu gösteren işaretçidir. Dördüncü parametre, kopyalama işleminin yapılacağı hedefin sonunu gösteren işaretçidir. İşlev, kopyalama işlemini gerçekleştirdikten sonra son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::copy_backward() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> src {1, 2, 3, 4, 5};
  std::vector<int> dest(src.size());

  std::copy_backward(src.begin(), src.end(), dest.end());

  for (auto it = dest.begin(); it != dest.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::copy_backward() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde src ve dest isimli iki vektör oluşturuyoruz. Ardından, std::copy_backward() işlevini kullanarak src vektöründeki öğeleri sondan başlayarak dest vektörüne kopyalıyoruz. Son olarak, dest vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğeleri sondan başlayarak başka bir aralığa taşımak için oldukça yaygındır. Örneğin, bir dosyada sondan başlayarak belirli bir karakter dizisi aramak veya bir veritabanında sondan başlayarak belirli bir sayıda kayıtları kopyalamak için kullanılabilir.

### move

- std::move() C++ algoritması, bir nesneyi taşımak (move) için kullanılır. Bu işlev, bir nesneyi başka bir nesneye atarken, kaynak nesnenin özelliklerinin çalınması (move) için kullanılır. Bu, özellikle büyük nesnelerin kopyalanması için zaman ve bellek kullanımı açısından daha verimli olabilir.

- std::move() işlevi, bir nesneyi taşımak için kullanılır. Bu işlev, bir nesnenin içeriğini değiştirmeden, sadece nesnenin sahipliğini başka bir nesneye aktarmak için kullanılır. Özellikle büyük veri yapıları ve nesnelerin kopyalanması için zaman ve bellek kullanımı açısından daha verimlidir.

- std::move() işlevi, C++11 ile birlikte standart kütüphaneye eklenmiştir ve utility başlık dosyasında tanımlanmıştır.

- İşte örnek bir kod parçası, std::move() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <utility>
#include <vector>

int main() {
  std::vector<int> src {1, 2, 3, 4, 5};
  std::vector<int> dest;

  dest = std::move(src);

  std::cout << "src vector size: " << src.size() << std::endl;
  std::cout << "dest vector size: " << dest.size() << std::endl;

  return 0;
}

```
> Bu örnek kod, std::move() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde src ve dest isimli iki vektör oluşturuyoruz. Ardından, std::move() işlevini kullanarak src vektörünü dest vektörüne taşıyoruz. Son olarak, src ve dest vektörlerinin boyutlarını yazdırıyoruz.

- Bu işlevin kullanımı, bir nesnenin sahipliğini transfer etmek için oldukça yaygındır. Örneğin, bir sınıf nesnesinin içeriğini başka bir sınıf nesnesine taşımak veya bir dizi büyük veri yapısını kopyalamak yerine, bunları taşımak için kullanılabilir.

### move_backward

- std::move_backward() C++ algoritması, bir aralıktaki öğeleri sondan başlayarak başka bir aralığa taşımak (move) için kullanılır. Bu işlev, bir nesnenin içeriğini değiştirmeden, sadece nesnenin sahipliğini başka bir nesneye aktarmak için kullanılır. Özellikle büyük veri yapıları ve nesnelerin taşınması için zaman ve bellek kullanımı açısından daha verimlidir.

- std::move_backward() işlevi, birinci ve ikinci parametre olarak taşınacak aralığın başlangıcını ve sonunu gösteren işaretçileri alır. Üçüncü parametre, taşınacak aralığın sonunu gösteren işaretçidir. Dördüncü parametre, taşıma işleminin yapılacağı hedefin sonunu gösteren işaretçidir. İşlev, taşıma işlemini gerçekleştirdikten sonra son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::move_backward() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> src {1, 2, 3, 4, 5};
  std::vector<int> dest(src.size());

  std::move_backward(src.begin(), src.end(), dest.end());

  std::cout << "src vector size: " << src.size() << std::endl;
  std::cout << "dest vector size: " << dest.size() << std::endl;

  return 0;
}

```
> Bu örnek kod, std::move_backward() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde src ve dest isimli iki vektör oluşturuyoruz. Ardından, std::move_backward() işlevini kullanarak src vektöründeki öğeleri sondan başlayarak dest vektörüne taşıyoruz. Son olarak, src ve dest vektörlerinin boyutlarını yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğeleri sondan başlayarak başka bir aralığa taşımak için oldukça yaygındır. Örneğin, bir dosyada sondan başlayarak belirli bir karakter dizisi aramak veya bir veritabanında sondan başlayarak belirli bir sayıda kayıtları taşımak için kullanılabilir.

### fill

- std::fill() C++ algoritması, bir aralığı belirli bir değerle doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir değerle kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::fill() işlevi, birinci ve ikinci parametre olarak doldurulacak aralığın başlangıcını ve sonunu gösteren işaretçileri alır. Üçüncü parametre, aralığın doldurulacağı değerdir. İşlev, belirtilen aralığı belirtilen değerle doldurduktan sonra son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::fill() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v(5);

  std::fill(v.begin(), v.end(), 42);

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::fill() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde v isimli bir vektör oluşturuyoruz. Ardından, std::fill() işlevini kullanarak v vektörünü 42 değeriyle dolduruyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığı belirli bir değerle doldurmak için oldukça yaygındır. Örneğin, bir dizi bellek bloğunu sıfırlamak veya bir veritabanındaki boş alanları belirli bir değerle doldurmak için kullanılabilir.

### fill_n()

- std::fill_n() C++ algoritması, bir aralığı belirli bir değerle belirli bir sayıda doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir değerle kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::fill_n() işlevi, birinci parametre olarak doldurulacak aralığın başlangıcını gösteren bir işaretçi alır. İkinci parametre, aralığın doldurulacak eleman sayısıdır. Üçüncü parametre, aralığın doldurulacağı değerdir. İşlev, belirtilen aralığı belirtilen değerle doldurduktan sonra son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::fill_n() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v(5);

  std::fill_n(v.begin(), 3, 42);

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::fill_n() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde v isimli bir vektör oluşturuyoruz. Ardından, std::fill_n() işlevini kullanarak v vektörünün ilk üç öğesini 42 değeriyle dolduruyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığı belirli bir değerle belirli bir sayıda doldurmak için oldukça yaygındır. Örneğin, bir bellek bloğunu belirli bir değerle sıfırlamak veya bir veritabanındaki boş alanları belirli bir değerle doldurmak için kullanılabilir.

### transform()

- std::transform() C++ algoritması, bir aralıktaki öğeleri başka bir aralığa dönüştürmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir işlemle değiştirerek başka bir aralığa aktarmak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::transform() işlevi, üç parametre alır. İlk iki parametre, dönüştürülecek aralığın başlangıcını ve sonunu gösteren işaretçilerdir. Üçüncü parametre, dönüştürülen öğelerin yazılacağı hedef aralığın başlangıcını gösteren bir işaretçidir. Dördüncü parametre, her öğe üzerinde uygulanacak dönüştürme işlevi olan bir fonksiyon nesnesidir. İşlev, dönüştürülen öğelerin yazıldığı son konumu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::transform() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2(v1.size());

  std::transform(v1.begin(), v1.end(), v2.begin(), [](int i) { return i * 2; });

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::transform() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 isimli bir vektör oluşturuyoruz. Ardından, v1 vektörünün boyutuna eşit bir v2 vektörü oluşturuyoruz. Sonra, std::transform() işlevini kullanarak v1 vektöründeki öğeleri iki katına çıkararak v2 vektörüne dönüştürüyoruz. Son olarak, v2 vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğeleri belirli bir işlemle dönüştürmek için oldukça yaygındır. Örneğin, bir dosyadaki karakterleri büyük harflere dönüştürmek veya bir dizi sayının karelerini hesaplamak için kullanılabilir.

### generate()

- std::generate() C++ algoritması, bir aralığı belirli bir işleme göre doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir işleme göre kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::generate() işlevi, iki parametre alır. İlk parametre, doldurulacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın doldurulacak son elemanının işaretçisidir. Üçüncü parametre, aralığı doldurmak için kullanılacak işlevdir. Bu işlev, aralığın her bir elemanı için çağrılır ve elemanın değeri bu işlevin dönüş değeri ile belirlenir. İşlev, doldurulan aralığın son konumunu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::generate() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v(5);

  std::generate(v.begin(), v.end(), []() { static int i = 0; return ++i; });

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::generate() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::generate() işlevini kullanarak v vektörünü sıralı sayılarla dolduruyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığı belirli bir işlemle doldurmak için oldukça yaygındır. Örneğin, bir dizi bellek bloğunu rastgele sayılarla doldurmak veya bir veritabanındaki boş alanları rastgele sayılarla doldurmak için kullanılabilir.

### generate_n()

- std::generate_n() C++ algoritması, bir aralığı belirli bir işleme göre belirli bir sayıda doldurmak için kullanılır. Bu algoritmanın amacı, bir aralığı belirli bir işleme göre kolayca doldurmak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::generate_n() işlevi, üç parametre alır. İlk parametre, doldurulacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, doldurulacak eleman sayısıdır. Üçüncü parametre, aralığı doldurmak için kullanılacak işlevdir. Bu işlev, aralığın her bir elemanı için çağrılır ve elemanın değeri bu işlevin dönüş değeri ile belirlenir. İşlev, doldurulan aralığın son konumunu gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::generate_n() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v(5);

  std::generate_n(v.begin(), 3, []() { static int i = 0; return ++i; });

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::generate_n() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::generate_n() işlevini kullanarak v vektörünün ilk üç öğesini sıralı sayılarla dolduruyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığı belirli bir işlemle belirli bir sayıda doldurmak için oldukça yaygındır. Örneğin, bir bellek bloğunu rastgele sayılarla doldurmak veya bir veritabanındaki boş alanları rastgele sayılarla doldurmak için kullanılabilir.

### remove()

- std::remove() C++ algoritması, bir aralıktaki öğelerden belirli bir değeri kaldırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir değere göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.

- std::remove() işlevi, iki parametre alır. İlk parametre, kaldırılacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, kaldırılacak değerin değeridir. İşlev, belirtilen değerle eşleşen tüm öğeleri aralığın sonuna taşıyarak aralığın yeni sonunu gösteren bir işaretçi döndürür.

- Ancak, bu işlev belirtilen değeri gerçekten aralıktan kaldırmaz, yalnızca aralıktan dışarı taşır. Bu nedenle, aralığın sonundan geriye doğru yeni aralık boyutunu hesaplamak ve aralığı bu boyuta yeniden boyutlandırmak için std::vector::erase() işlevi kullanılmalıdır.

- İşte örnek bir kod parçası, std::remove() ve std::vector::erase() işlevlerinin nasıl kullanılabileceğini gösteriyo

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 2, 4, 2, 5};

  auto new_end = std::remove(v.begin(), v.end(), 2);
  v.erase(new_end, v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::remove() ve std::vector::erase() işlevlerinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::remove() işlevini kullanarak v vektöründeki tüm 2 değerlerini kaldırıyoruz ve aralığın yeni sonunu gösteren bir işaretçi elde ediyoruz. Son olarak, std::vector::erase() işlevini kullanarak aralığı yeniden boyutlandırıyoruz ve v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki belirli bir değeri kaldırmak veya değiştirmek için oldukça yaygındır. Örneğin, bir dizi karakterden belirli bir karakteri kaldırmak veya bir dizi sayıdan belirli bir sayıyı değiştirmek için kullanılabilir.

### remove_if()

- std::remove_if() C++ algoritması, bir aralıktaki öğelerden belirli bir koşulu sağlayanları kaldırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.

- std::remove_if() işlevi, iki parametre alır. İlk parametre, kaldırılacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, kaldırılacak öğelerin belirlenmesi için kullanılacak koşulu tanımlayan bir fonksiyon nesnesidir. İşlev, belirtilen koşulu sağlayan tüm öğeleri aralığın sonuna taşıyarak aralığın yeni sonunu gösteren bir işaretçi döndürür.

- Ancak, bu işlev belirtilen öğeleri gerçekten aralıktan kaldırmaz, yalnızca aralıktan dışarı taşır. Bu nedenle, aralığın sonundan geriye doğru yeni aralık boyutunu hesaplamak ve aralığı bu boyuta yeniden boyutlandırmak için std::vector::erase() işlevi kullanılmalıdır.

- İşte örnek bir kod parçası, std::remove_if() ve std::vector::erase() işlevlerinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int n) {
  return n % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

  auto new_end = std::remove_if(v.begin(), v.end(), is_even);
  v.erase(new_end, v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::remove_if() ve std::vector::erase() işlevlerinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::remove_if() işlevini kullanarak v vektöründeki tüm çift sayıları kaldırıyoruz ve aralığın yeni sonunu gösteren bir işaretçi elde ediyoruz. Son olarak, std::vector::erase() işlevini kullanarak aralığı yeniden boyutlandırıyoruz ve v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki belirli bir koşulu sağlayan öğeleri kaldırmak veya değiştirmek için oldukça yaygındır. Örneğin, bir karakter dizisinden belirli bir karakteri kaldırmak veya bir dizi sayıdan belirli bir koşulu sağlayan öğeleri kaldırmak için kullanılabilir.

### remove_copy()

- std::remove_copy() C++ algoritması, bir aralıktan belirli bir öğeyi kaldırarak yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca kopyalamak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::remove_copy() işlevi, üç parametre alır. İlk parametre, kopyalanacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, kopyalanacak aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, kaldırılacak öğenin değeridir. Dördüncü parametre, yeni aralığın başlangıcını gösteren bir işaretçidir. İşlev, belirtilen öğeyi kaldırarak yeni aralığı oluşturur ve yeni aralığın sonunu gösteren bir işaretçi döndürür.

- std::remove_copy() işlevi, orijinal aralığı değiştirmez. Bunun yerine, yeni bir aralık oluşturur ve orijinal aralığın değerlerini bu aralığa kopyalar. Bu nedenle, orijinal aralık ve yeni aralık farklı olabilir.

- İşte örnek bir kod parçası, std::remove_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 2, 4, 2, 5};
  std::vector<int> v2(v.size());

  std::remove_copy(v.begin(), v.end(), v2.begin(), 2);

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::remove_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::remove_copy() işlevini kullanarak v vektöründeki tüm 2 değerlerini kaldırarak yeni bir vektör oluşturuyoruz. Son olarak, yeni vektördeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktan belirli bir öğeyi kaldırarak yeni bir aralık oluşturmak için oldukça yaygındır. Örneğin, bir karakter dizisinden belirli bir karakteri kaldırmak veya bir dizi sayıdan belirli bir koşulu sağlayan öğeleri kaldırmak için kullanılabilir.

### remove_copy_if()

- std::remove_copy_if() C++ algoritması, bir aralıktan belirli bir koşulu sağlayan öğeleri kaldırarak yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca kopyalamak ve bu işlemi hızlı bir şekilde yapmaktır.

- std::remove_copy_if() işlevi, dört parametre alır. İlk parametre, kopyalanacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, kopyalanacak aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, kaldırılacak öğelerin belirlenmesi için kullanılacak koşulu tanımlayan bir fonksiyon nesnesidir. Dördüncü parametre, yeni aralığın başlangıcını gösteren bir işaretçidir. İşlev, belirtilen koşulu sağlayan öğeleri kaldırarak yeni aralığı oluşturur ve yeni aralığın sonunu gösteren bir işaretçi döndürür.

- std::remove_copy_if() işlevi, orijinal aralığı değiştirmez. Bunun yerine, yeni bir aralık oluşturur ve orijinal aralığın değerlerini bu aralığa kopyalar. Bu nedenle, orijinal aralık ve yeni aralık farklı olabilir.

- İşte örnek bir kod parçası, std::remove_copy_if() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int n) {
  return n % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
  std::vector<int> v2(v.size());

  std::remove_copy_if(v.begin(), v.end(), v2.begin(), is_even);

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::remove_copy_if() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::remove_copy_if() işlevini kullanarak v vektöründeki tüm çift sayıları kaldırarak yeni bir vektör oluşturuyoruz. Son olarak, yeni vektördeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktan belirli bir koşulu sağlayan öğeleri kaldırarak yeni bir aralık oluşturmak için oldukça yaygındır. Örneğin, bir karakter dizisinden belirli bir karakteri kaldırmak veya bir dizi sayıdan belirli bir koşulu sağlayan öğeleri kaldırmak için kullanılabilir.

### replace()

- std::replace() C++ algoritması, bir aralıktaki belirli bir değeri başka bir değerle değiştirmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir değere göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.

- std::replace() işlevi, üç parametre alır. İlk parametre, değiştirilecek aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, değiştirilecek aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, değiştirilecek öğenin değeridir. Dördüncü parametre, öğelerin değiştirileceği yeni değeri gösteren bir değerdir. İşlev, belirtilen değere sahip tüm öğeleri yeni değerle değiştirir.

- std::replace() işlevi, orijinal aralığı değiştirir. Bu nedenle, orijinal aralık değiştirilmeden önce yedeklenmelidir.

- İşte örnek bir kod parçası, std::replace() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};

  std::replace(v.begin(), v.end(), 3, 6);

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::replace() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::replace() işlevini kullanarak v vektöründeki tüm 3 değerlerini 6 ile değiştiriyoruz. Son olarak, vektördeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki belirli bir değeri başka bir değerle değiştirmek için oldukça yaygındır. Örneğin, bir karakter dizisindeki belirli bir karakteri başka bir karakterle değiştirmek veya bir dizi sayıdaki belirli bir değeri başka bir değerle değiştirmek için kullanılabilir.

### replace_if()

- std::replace_if() C++ algoritması, bir aralıktaki belirli bir koşulu sağlayan öğeleri başka bir değerle değiştirmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.

- std::replace_if() işlevi, dört parametre alır. İlk parametre, değiştirilecek aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, değiştirilecek aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, öğelerin değiştirilip değiştirilmeyeceğini belirlemek için kullanılacak koşulu tanımlayan bir fonksiyon nesnesidir. Dördüncü parametre, öğelerin değiştirileceği yeni değeri gösteren bir değerdir. İşlev, belirtilen koşulu sağlayan tüm öğeleri yeni değerle değiştirir.

- std::replace_if() işlevi, orijinal aralığı değiştirir. Bu nedenle, orijinal aralık değiştirilmeden önce yedeklenmelidir.

- İşte örnek bir kod parçası, std::replace_if() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int n) {
  return n % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};

  std::replace_if(v.begin(), v.end(), is_even, 0);

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::replace_if() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::replace_if() işlevini kullanarak v vektöründeki tüm çift sayıları 0 ile değiştiriyoruz. Son olarak, vektördeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki belirli bir koşulu sağlayan öğeleri başka bir değerle değiştirmek için oldukça yaygındır. Örneğin, bir karakter dizisindeki belirli bir karakterleri başka bir karakterle değiştirmek veya bir dizi sayıdaki belirli bir koşulu sağlayan değerleri başka bir değerle değiştirmek için kullanılabilir.

### replace_copy()
- std::replace_copy() C++ algoritması, bir aralıktan belirli bir değeri başka bir değerle değiştirerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir değere göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.

- std::replace_copy() işlevi, dört parametre alır. İlk parametre, kopyalanacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, kopyalanacak aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, değiştirilecek öğenin değeridir. Dördüncü parametre, öğelerin değiştirileceği yeni değeri gösteren bir değerdir. Beşinci parametre, yeni aralığın başlangıcını gösteren bir işaretçidir. İşlev, belirtilen değere sahip tüm öğeleri yeni değerle değiştirerek yeni aralığı oluşturur ve yeni aralığın sonunu gösteren bir işaretçi döndürür.

- std::replace_copy() işlevi, orijinal aralığı değiştirmez. Bunun yerine, yeni bir aralık oluşturur ve orijinal aralığın değerlerini bu aralığa kopyalar. Bu nedenle, orijinal aralık ve yeni aralık farklı olabilir.

- İşte örnek bir kod parçası, std::replace_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};
  std::vector<int> v2(v.size());

  std::replace_copy(v.begin(), v.end(), v2.begin(), 3, 6);

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::replace_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde v isimli bir vektör oluşturuyoruz. Ardından, std::replace_copy() işlevini kullanarak v vektöründeki tüm 3 değerlerini 6 ile değiştirerek yeni bir vektör oluşturuyoruz. Son olarak, yeni vektördeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki belirli bir değeri başka bir değerle değiştirerek yeni bir aralık oluşturmak için oldukça yaygındır. Örneğin, bir karakter dizisindeki belirli bir karakterleri başka bir karakterle değiştirerek yeni bir karakter dizisi oluşturmak veya bir dizi sayıdaki belirli bir değeri başka bir değerle değiştirerek yeni bir dizi oluşturmak için kullanılabilir.

### replace_copy_if()
- std::replace_copy_if() C++ algoritması, bir aralıktan belirli bir koşulu sağlayan öğeleri başka bir değerle değiştirerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir koşula göre kolayca değiştirmek ve bu işlemi hızlı bir şekilde yapmaktır.

- std::replace_copy_if() işlevi, beş parametre alır. İlk parametre, kopyalanacak aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, kopyalanacak aralığın sonunu gösteren bir işaretçidir. Üçüncü parametre, öğelerin değiştirilip değiştirilmeyeceğini belirlemek için kullanılacak koşulu tanımlayan bir fonksiyon nesnesidir. Dördüncü parametre, öğelerin değiştirileceği yeni değeri gösteren bir değerdir. Beşinci parametre, yeni aralığın başlangıcını gösteren bir işaretçidir. İşlev, belirtilen koşulu sağlayan tüm öğeleri yeni değerle değiştirerek yeni aralığı oluşturur ve yeni aralığın sonunu gösteren bir işaretçi döndürür.

- std::replace_copy_if() işlevi, orijinal aralığı değiştirmez. Bunun yerine, yeni bir aralık oluşturur ve orijinal aralığın değerlerini bu aralığa kopyalar. Bu nedenle, orijinal aralık ve yeni aralık farklı olabilir.

- İşte örnek bir kod parçası, std::replace_copy_if() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int n) {
  return n % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};
  std::vector<int> v2(v.size());

  std::replace_copy_if(v.begin(), v.end(), v2.begin(), is_even, 0);

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::replace_copy_if() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde v isimli bir vektör oluşturuyoruz. Ardından, std::replace_copy_if() işlevini kullanarak v vektöründeki tüm çift sayıları 0 ile değiştirerek yeni bir vektör oluşturuyoruz. Son olarak, yeni vektördeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki belirli bir koşulu sağlayan öğeleri başka bir değerle değiştirerek yeni bir aralık oluşturmak oldukça yaygındır. Örneğin, bir karakter dizisindeki belirli bir karakterleri başka bir karakterle değiştirerek yeni bir karakter dizisi oluşturmak veya bir dizi sayıdaki belirli bir koşulu sağlayan değerleri başka bir değerle değiştirerek yeni bir dizi oluşturmak için kullanılabilir.

### swap()
- std::swap() C++ algoritması, iki nesnenin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki nesnenin değerlerini hızlı bir şekilde değiştirmektir.

- std::swap() işlevi, iki referans parametre alır ve bu parametrelerin değerlerini değiştirir. Bu işlev, C++ standart kütüphanesi tarafından sağlanır ve nesnelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::swap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>

int main() {
  int a = 10, b = 20;

  std::cout << "a: " << a << " b: " << b << std::endl;

  std::swap(a, b);

  std::cout << "a: " << a << " b: " << b << std::endl;

  return 0;
}

```
> Bu örnek kod, std::swap() işlevinin kullanımını göstermektedir. İlk olarak, a ve b olmak üzere iki tamsayı değişkeni tanımlıyoruz. Ardından, std::swap() işlevini kullanarak a ve b değişkenlerinin değerlerini değiştiriyoruz. Son olarak, a ve b değişkenlerinin yeni değerlerini yazdırıyoruz.

- Bu işlevin kullanımı, özellikle sıralama ve diğer algoritmalarla birlikte kullanıldığında oldukça yaygındır. Örneğin, bir vektördeki iki öğenin yerini değiştirmek veya iki karakter dizisini yer değiştirmek için kullanılabilir.

### swap_ranges

- std::swap_ranges() C++ algoritması, iki aralıktaki öğelerin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki aralıktaki öğelerin değerlerini hızlı bir şekilde değiştirmektir.

- std::swap_ranges() işlevi, iki aralık ve bunların başlangıç konumlarını gösteren iki işaretçi parametre alır. İşlev, iki aralık arasındaki öğelerin değerlerini tek tek değiştirerek bu işlemi gerçekleştirir. İşlev, değiştirilen son öğenin ardından ikinci aralığın başlangıcını gösteren bir işaretçi döndürür.

- İşte örnek bir kod parçası, std::swap_ranges() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {6, 7, 8, 9, 10};

  std::swap_ranges(v1.begin(), v1.begin() + 3, v2.begin() + 2);

  for (auto it = v1.begin(); it != v1.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```

> Bu örnek kod, std::swap_ranges() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz. Ardından, std::swap_ranges() işlevini kullanarak v1 vektörünün ilk üç öğesini v2 vektörünün üçüncü öğesinden başlayarak değiştiriyoruz. Son olarak, v1 ve v2 vektörlerindeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, iki aralıktaki öğelerin değerlerini değiştirerek yeni bir aralık oluşturmak için oldukça yaygındır. Örneğin, iki karakter dizisindeki öğelerin yerini değiştirmek için kullanılabilir.

### iter_swap()

- std::iter_swap() C++ algoritması, iki nesnenin değerlerini değiştirmek için kullanılır. Bu algoritmanın amacı, iki nesnenin değerlerini hızlı bir şekilde değiştirmektir.

- std::iter_swap() işlevi, iki işaretçi parametre alır ve bu parametrelerin gösterdiği iki nesnenin değerlerini değiştirir. Bu işlev, C++ standart kütüphanesi tarafından sağlanır ve nesnelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::iter_swap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};

  std::iter_swap(v.begin(), v.begin() + 3);

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```

> Bu örnek kod, std::iter_swap() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::iter_swap() işlevini kullanarak v vektöründeki ilk öğe ile dördüncü öğenin yerlerini değiştiriyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle sıralama ve diğer algoritmalarla birlikte kullanıldığında oldukça yaygındır. Örneğin, bir vektördeki iki öğenin yerini değiştirmek veya iki karakter dizisini yer değiştirmek için kullanılabilir.

### reverse

- std::reverse() C++ algoritması, bir aralıktaki öğelerin sırasını tersine çevirmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin sırasını hızlı bir şekilde tersine çevirmektir.

- std::reverse() işlevi, bir aralık ve bunun başlangıç konumunu gösteren iki işaretçi parametre alır. İşlev, aralıktaki öğelerin sırasını tersine çevirerek bu işlemi gerçekleştirir.

- İşte örnek bir kod parçası, std::reverse() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};

  std::reverse(v.begin(), v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::reverse() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::reverse() işlevini kullanarak v vektöründeki öğelerin sırasını tersine çeviriyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle ters sıralama yapmak ve ters diziler oluşturmak için oldukça yaygındır. Örneğin, bir karakter dizisini ters çevirmek veya bir matrisin sütunlarını tersine çevirmek için kullanılabilir.

### reverse_copy()

- std::reverse_copy() C++ algoritması, bir aralıktaki öğelerin sırasını tersine çevirerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin sırasını hızlı bir şekilde tersine çevirerek yeni bir aralık oluşturmaktır.

- std::reverse_copy() işlevi, bir aralık ve bunun başlangıç konumunu gösteren iki işaretçi parametre ile hedef aralığın başlangıç konumunu gösteren bir işaretçi parametre alır. İşlev, kaynak aralıktaki öğelerin sırasını tersine çevirerek hedef aralıkta yeni bir aralık oluşturur.

- İşte örnek bir kod parçası, std::reverse_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};
  std::vector<int> v_reverse(v.size());

  std::reverse_copy(v.begin(), v.end(), v_reverse.begin());

  for (auto it = v_reverse.begin(); it != v_reverse.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::reverse_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, v_reverse isimli bir başka vektör oluşturuyoruz ve std::reverse_copy() işlevini kullanarak v vektörünü tersine çevirerek v_reverse vektörüne kopyalıyoruz. Son olarak, v_reverse vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle ters sıralama yaparak yeni bir aralık oluşturmak ve ters diziler oluşturmak için oldukça yaygındır. Örneğin, bir karakter dizisini ters çevirerek yeni bir karakter dizisi oluşturmak veya bir matrisin sütunlarını tersine çevirerek yeni bir matris oluşturmak için kullanılabilir.

### rotate

- std::rotate() C++ algoritması, bir aralıktaki öğeleri belirli bir konuma kadar döndürmek için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin belirli bir konuma kadar döndürülmesini sağlamaktır.

- std::rotate() işlevi, bir aralık ve dönüşümün başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen konuma kadar olan öğeleri aralığın sonuna taşır ve belirtilen konumda öğelerin yeni başlangıcını belirler. Bu işlem, döndürülen öğelerin sayısı ve aralıktaki öğelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::rotate() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};

  std::rotate(v.begin(), v.begin() + 3, v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::rotate() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::rotate() işlevini kullanarak v vektöründeki öğeleri üçüncü öğeden başlayarak döndürüyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir konuma kadar döndürülmesi gerektiğinde oldukça yaygındır. Örneğin, bir karakter dizisini belirli bir konuma kadar döndürmek veya bir matrisin satırlarını döndürmek için kullanılabilir.

### rotate_copy

- std::rotate_copy() C++ algoritması, bir aralıktaki öğeleri belirli bir konuma kadar döndürerek yeni bir aralık oluşturmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğelerin belirli bir konuma kadar döndürülmesini sağlayarak yeni bir aralık oluşturmaktır.

- std::rotate_copy() işlevi, bir aralık, dönüşümün başlangıç konumunu gösteren bir işaretçi parametresi ve hedef aralığın başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen konuma kadar olan öğeleri aralığın sonuna taşır ve belirtilen konumda öğelerin yeni başlangıcını belirler. Bu işlem, döndürülen öğelerin sayısı ve aralıktaki öğelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::rotate_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};
  std::vector<int> v_rotated(v.size());

  std::rotate_copy(v.begin(), v.begin() + 3, v.end(), v_rotated.begin());

  for (auto it = v_rotated.begin(); it != v_rotated.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::rotate_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, v_rotated isimli bir başka vektör oluşturuyoruz ve std::rotate_copy() işlevini kullanarak v vektöründeki öğeleri üçüncü öğeden başlayarak döndürerek v_rotated vektörüne kopyalıyoruz. Son olarak, v_rotated vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir konuma kadar döndürülerek yeni bir aralık oluşturulması gerektiğinde oldukça yaygındır. Örneğin, bir karakter dizisini belirli bir konuma kadar döndürerek yeni bir karakter dizisi oluşturmak veya bir matrisin satırlarını döndürerek yeni bir matris oluşturmak için kullanılabilir.

### shift_left()

- std::shift_left() C++20 algoritması, bir aralıktaki öğeleri belirli bir sayıda sol tarafa kaydırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir sayıda sola kaydırarak yeni bir aralık oluşturmaktır.

- std::shift_left() işlevi, bir aralık, kaydırma miktarını gösteren bir sayı ve hedef aralığın başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen sayıda öğeyi sola kaydırarak hedef aralıkta yeni bir aralık oluşturur. Bu işlem, kaydırılan öğelerin sayısı ve aralıktaki öğelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::shift_left() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};
  std::vector<int> v_shifted(v.size());

  std::shift_left(v.begin(), v.end(), 2, v_shifted.begin());

  for (auto it = v_shifted.begin(); it != v_shifted.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::shift_left() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, v_shifted isimli bir başka vektör oluşturuyoruz ve std::shift_left() işlevini kullanarak v vektöründeki öğeleri iki adet sola kaydırarak v_shifted vektörüne kopyalıyoruz. Son olarak, v_shifted vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir sayıda sola kaydırılması gerektiğinde oldukça yaygındır. Örneğin, bir karakter dizisini belirli bir sayıda sola kaydırmak veya bir matrisin sütunlarını belirli bir sayıda sola kaydırmak için kullanılabilir.

### shift_right

- std::shift_right() C++20 algoritması, bir aralıktaki öğeleri belirli bir sayıda sağ tarafa kaydırmak için kullanılır. Bu algoritmanın amacı, bir aralıktaki öğeleri belirli bir sayıda sağa kaydırarak yeni bir aralık oluşturmaktır.

- std::shift_right() işlevi, bir aralık, kaydırma miktarını gösteren bir sayı ve hedef aralığın başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen sayıda öğeyi sağa kaydırarak hedef aralıkta yeni bir aralık oluşturur. Bu işlem, kaydırılan öğelerin sayısı ve aralıktaki öğelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::shift_right() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};
  std::vector<int> v_shifted(v.size());

  std::shift_right(v.begin(), v.end(), 2, v_shifted.begin());

  for (auto it = v_shifted.begin(); it != v_shifted.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```

> Bu örnek kod, std::shift_right() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, v_shifted isimli bir başka vektör oluşturuyoruz ve std::shift_right() işlevini kullanarak v vektöründeki öğeleri iki adet sağa kaydırarak v_shifted vektörüne kopyalıyoruz. Son olarak, v_shifted vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir sayıda sağa kaydırılması gerektiğinde oldukça yaygındır. Örneğin, bir karakter dizisini belirli bir sayıda sağa kaydırmak veya bir matrisin sütunlarını belirli bir sayıda sağa kaydırmak için kullanılabilir.

### shuffle

- std::shuffle() C++20 algoritması, bir aralıktaki öğeleri rastgele bir sıraya yerleştirir. Bu algoritmanın amacı, bir aralıktaki öğelerin rastgele bir sıraya yerleştirilmesidir.

- std::shuffle() işlevi, bir aralık, rastgele sayı üreteci, hedef aralığın başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğeleri rastgele bir şekilde karıştırarak hedef aralıkta yeni bir aralık oluşturur. Bu işlem, karıştırılacak öğelerin sayısı, kullanılacak rastgele sayı üretecinin türü ve aralıktaki öğelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::shuffle() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>
#include <random>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5};

  std::random_device rd;
  std::mt19937 g(rd());
  std::shuffle(v.begin(), v.end(), g);

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```

> Bu örnek kod, std::shuffle() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, rastgele sayı üreteci için bir std::mt19937 nesnesi oluşturuyoruz ve std::shuffle() işlevini kullanarak v vektöründeki öğeleri rastgele bir şekilde karıştırıyoruz. Son olarak, v vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin rastgele bir sıraya yerleştirilmesi gerektiğinde oldukça yaygındır. Örneğin, bir kart destesini karıştırmak veya bir dizi sayıyı rastgele bir sıraya yerleştirmek için kullanılabilir.

### sample

- std::sample() C++17'de eklenen bir algoritmadır ve bir aralıktan belirli bir sayıda öğeyi rastgele örneklemek için kullanılır.

std::sample() işlevi, bir aralık, örneklem boyutu, rastgele sayı üreteci, hedef aralığın başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen aralıktan rastgele öğeler seçerek hedef aralıkta yeni bir aralık oluşturur. Bu işlem, örneklem boyutu ve aralıktaki öğelerin türüne göre özelleştirilebilir.

İşte örnek bir kod parçası, std::sample() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>
#include <random>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
  std::vector<int> sample(5);

  std::random_device rd;
  std::mt19937 g(rd());
  std::sample(v.begin(), v.end(), sample.begin(), 5, g);

  for (auto it = sample.begin(); it != sample.end(); ++it) {
    std::cout << *it << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::sample() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, sample isimli başka bir vektör oluşturuyoruz ve std::sample() işlevini kullanarak v vektöründen beş adet rastgele öğe seçiyoruz. Son olarak, seçilen öğeleri sample vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktan belirli bir sayıda öğe örneklemek gerektiğinde oldukça yaygındır. Örneğin, bir reklam kampanyası için bir müşteri örnekleminin seçilmesi veya bir popülasyon örnekleminin analiz edilmesi için kullanılabilir.

### unique()

- std::unique() algoritması, bir aralıktaki ardışık tekrarlayan öğeleri kaldırır ve ardışık olmayan tekrarlayan öğelerin bir kopyasını yeni bir aralıkta oluşturur.

- Bu algoritma, bir aralıktaki öğelerin benzersiz hale getirilmesi gerektiğinde sıklıkla kullanılır. Örneğin, bir dizi sayıdaki yinelenen öğelerin kaldırılması veya bir cümle içindeki yinelenen kelimelerin kaldırılması gibi durumlarda kullanılabilir.

- std::unique() işlevi, bir aralık ve hedef aralığın başlangıç konumunu gösteren bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğelerden ardışık olarak tekrarlananları kaldırır ve hedef aralıkta yeni bir aralık oluşturur. Bu işlem, kopyalanan öğelerin türüne ve hedef aralıktaki öğelerin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::unique() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 2, 3, 3, 3, 4, 4, 4, 4};

  auto it = std::unique(v.begin(), v.end());

  for (auto i = v.begin(); i != it; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::unique() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::unique() işlevini kullanarak v vektöründeki tekrarlayan öğeleri kaldırıyoruz. Son olarak, kopyalanan benzersiz öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki ardışık tekrarlayan öğelerin kaldırılması gerektiğinde oldukça yaygındır.

### unique_copy()

- std::unique_copy() algoritması, bir aralıktaki ardışık tekrarlayan öğeleri kaldırır ve ardışık olmayan tekrarlayan öğelerin bir kopyasını yeni bir aralıkta oluşturur. std::unique() işlevine benzer, ancak farklı olarak, std::unique_copy() işlevi, kopyalanan benzersiz öğeleri yeni bir aralığa yerleştirir, orijinal aralığı değiştirmez.

- Bu algoritma, bir aralıktaki öğelerin benzersiz hale getirilmesi ve kopyalanması gerektiğinde sıklıkla kullanılır. Örneğin, bir dizi sayıdaki yinelenen öğelerin kaldırılması ve kopyalanması veya bir cümle içindeki yinelenen kelimelerin kaldırılması ve kopyalanması gibi durumlarda kullanılabilir.

- std::unique_copy() işlevi, bir aralık, hedef aralık ve eşsiz öğelerin karşılaştırılması için bir işlev veya işlev nesnesi parametresi alır. İşlev, belirtilen aralıktaki öğelerden ardışık olarak tekrarlananları kaldırır ve hedef aralıkta yeni bir aralık oluşturur. Bu işlem, kopyalanan öğelerin türüne, hedef aralıktaki öğelerin türüne ve eşsizlik testi için kullanılan işlevin türüne göre özelleştirilebilir.

- İşte örnek bir kod parçası, std::unique_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 2, 3, 3, 3, 4, 4, 4, 4};
  std::vector<int> v2;

  std::unique_copy(v.begin(), v.end(), std::back_inserter(v2));

  for (auto i = v2.begin(); i != v2.end(); ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::unique_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::unique_copy() işlevini kullanarak v vektöründeki tekrarlayan öğeleri kaldırıp kopyalıyoruz. Son olarak, kopyalanan benzersiz öğeleri yeni bir vektöre yerleştiriyoruz ve bu öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki ardışık tekrarlayan öğelerin kaldırılması ve kopyalanması gerektiğinde oldukça yaygındır.

### is_partitioned

- std::is_partitioned() işlevi, belirtilen aralıkta öğelerin belirli bir ölçüte göre bölünüp bölünmediğini kontrol eder.

- Bu algoritma, bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması gerektiğinde sıklıkla kullanılır. Örneğin, bir listedeki çift sayıların tek sayılardan ayrılması gibi durumlarda kullanılabilir.

- std::is_partitioned() işlevi, bir aralık ve bölme noktası için bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğelerin belirtilen ölçüte göre bölünüp bölünmediğini kontrol eder ve bool türünde bir değer döndürür.

- İşte örnek bir kod parçası, std::is_partitioned() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int i) {
  return i % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

  auto it = std::partition(v.begin(), v.end(), is_even);

  bool result = std::is_partitioned(v.begin(), v.end(), is_even);

  std::cout << std::boolalpha << result << std::endl;

  return 0;
}

```

> Bu örnek kod, std::is_partitioned() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::partition() işlevini kullanarak v vektöründeki çift sayıları önce, sonra da tek sayıları yerleştiriyoruz. Son olarak, std::is_partitioned() işlevini kullanarak, v vektöründeki öğelerin belirtilen ölçüte göre bölünüp bölünmediğini kontrol ediyoruz ve sonucu yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması gerektiğinde oldukça yaygındır.

### partition

- std::partition() işlevi, bir aralıktaki öğeleri belirli bir ölçüte göre bölerek, ölçüye uyan öğeleri bir tarafa yerleştirir ve uymayanları diğer tarafa yerleştirir. Bu işlev, bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması gerektiğinde sıklıkla kullanılır. Örneğin, bir listedeki çift sayıların tek sayılardan ayrılması gibi durumlarda kullanılabilir.

- std::partition() işlevi, bir aralık ve bölme noktası için bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğeleri belirtilen ölçüte göre bölerek, ölçüye uyan öğeleri aralığın baş tarafına, uymayan öğeleri ise aralığın son tarafına yerleştirir.

- İşte örnek bir kod parçası, std::partition() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int i) {
  return i % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

  auto it = std::partition(v.begin(), v.end(), is_even);

  std::cout << "Evens: ";
  for (auto i = v.begin(); i != it; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  std::cout << "Odds: ";
  for (auto i = it; i != v.end(); ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::partition() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::partition() işlevini kullanarak v vektöründeki çift sayıları önce, sonra da tek sayıları yerleştiriyoruz. Son olarak, çift ve tek sayıları ayrı ayrı yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması gerektiğinde oldukça yaygındır.

### partition_copy()

- std::partition_copy() işlevi, bir aralıktaki öğeleri belirli bir ölçüte göre böler ve iki farklı aralıkta sonuçları saklar. Ölçüye uyan öğeleri birinci aralığa, uymayan öğeleri ikinci aralığa kopyalar. Bu işlev, bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması ve sonuçların ayrı ayrı saklanması gerektiğinde sıklıkla kullanılır.

- std::partition_copy() işlevi, bir kaynak aralığı, hedef aralıklarını, ve bölme noktası için bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğeleri belirtilen ölçüte göre böler ve sonuçları iki farklı aralıkta saklar.

- İşte örnek bir kod parçası, std::partition_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int i) {
  return i % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
  std::vector<int> evens(v.size());
  std::vector<int> odds(v.size());

  auto it = std::partition_copy(v.begin(), v.end(), evens.begin(), odds.begin(), is_even);

  std::cout << "Evens: ";
  for (auto i = evens.begin(); i != it.first; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  std::cout << "Odds: ";
  for (auto i = odds.begin(); i != it.second; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::partition_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::partition_copy() işlevini kullanarak v vektöründeki çift sayıları önce, sonra da tek sayıları yerleştiriyoruz. Son olarak, çift ve tek sayıları ayrı ayrı yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir ölçüte göre ayrılması ve sonuçların ayrı ayrı saklanması gerektiğinde oldukça yaygındır.

### stable_partition()

- std::stable_partition() işlevi, bir aralıktaki öğeleri belirli bir ölçüte göre böler ve ölçüye uyan öğeleri bir tarafa yerleştirir, uymayan öğeleri ise diğer tarafa yerleştirir. Bu işlev, std::partition() işlevi ile aynı işi yapar ancak sırayı korur. Bu nedenle, bu işlev, özellikle sıra önemli olduğunda kullanılır.

- std::stable_partition() işlevi, bir aralık ve bölme noktası için bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğeleri belirtilen ölçüte göre böler ve ölçüye uyan öğeleri aralığın baş tarafına, uymayan öğeleri ise aralığın son tarafına yerleştirir. Bu işlem sırasında, öğelerin özgün sıraları korunur.

- İşte örnek bir kod parçası, std::stable_partition() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int i) {
  return i % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

  std::stable_partition(v.begin(), v.end(), is_even);

  for (auto i : v) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::stable_partition() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::stable_partition() işlevini kullanarak v vektöründeki çift sayıları önce, sonra da tek sayıları yerleştiriyoruz. Son olarak, vektörü yazdırıyoruz.

- Bu işlevin kullanımı, özellikle sıra önemli olduğunda ve özgün sıralamanın korunması gerektiğinde oldukça yaygındır.

### partition_point

- std::partition_point() işlevi, bir aralıktaki öğeleri belirli bir ölçüte göre böldükten sonra, bölme noktasını belirlemek için kullanılır. Bölme noktası, ölçüye uymayan öğelerin başladığı noktadır. Bu işlev, özellikle std::partition() işleviyle birlikte kullanıldığında faydalıdır.

- std::partition_point() işlevi, bir aralık ve bölme noktası için bir işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğeleri belirtilen ölçüte göre böler ve bölme noktasını hesaplar.

- İşte örnek bir kod parçası, std::partition_point() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

bool is_even(int i) {
  return i % 2 == 0;
}

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

  auto it = std::partition(v.begin(), v.end(), is_even);

  std::cout << "First odd element: " << *std::partition_point(v.begin(), v.end(), is_even) << std::endl;

  return 0;
}

```

> Bu örnek kod, std::partition_point() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::partition() işlevini kullanarak v vektöründeki çift sayıları önce, sonra da tek sayıları yerleştiriyoruz. Son olarak, std::partition_point() işlevini kullanarak bölme noktasını buluyoruz ve ilk tek sayıyı yazdırıyoruz.

- Bu işlevin kullanımı, özellikle std::partition() işlevi ile birlikte kullanıldığında oldukça faydalıdır ve bir aralıktaki öğelerin belirli bir ölçüte göre bölündükten sonra hangi noktada bölündüğünü bulmak gerektiğinde kullanılabilir.

### is_sorted()

- std::is_sorted() işlevi, bir aralıktaki öğelerin belirli bir sıraya göre sıralanıp sıralanmadığını kontrol eder. Eğer belirtilen aralıktaki öğeler belirtilen sıraya göre sıralanmışsa, işlev true değerini döndürür. Aksi takdirde, false değerini döndürür.

- std::is_sorted() işlevi, bir aralık için iki adet işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğelerin sıralanma durumunu kontrol eder.

- İşte örnek bir kod parçası, std::is_sorted() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5, 6};
  std::vector<int> v2 {1, 3, 2, 4, 5, 6};

  std::cout << std::boolalpha;
  std::cout << "v1 is sorted: " << std::is_sorted(v1.begin(), v1.end()) << std::endl;
  std::cout << "v2 is sorted: " << std::is_sorted(v2.begin(), v2.end()) << std::endl;

  return 0;
}

```
> Bu örnek kod, std::is_sorted() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz. Ardından, std::is_sorted() işlevini kullanarak v1 ve v2 vektörlerinin sıralı olup olmadığını kontrol ediyoruz. Son olarak, her iki vektörün sıralı olup olmadığını yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir sıraya göre sıralanmış olup olmadığını kontrol etmek gerektiğinde oldukça yaygındır.

### is_sorted_until()

- std::is_sorted_until() işlevi, bir aralıktaki öğelerin belirli bir sıraya göre sıralanmış olduğu son öğenin işaretçisini döndürür. Bu işlev, std::is_sorted() işlevine benzerdir ancak sıralı olan öğelerin sonuncusunu işaret eder.

- std::is_sorted_until() işlevi, bir aralık için iki adet işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğelerin sıralanma durumunu kontrol eder ve sıralı olan son öğenin işaretçisini döndürür.

- İşte örnek bir kod parçası, std::is_sorted_until() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5, 6};
  std::vector<int> v2 {1, 3, 2, 4, 5, 6};

  auto it1 = std::is_sorted_until(v1.begin(), v1.end());
  auto it2 = std::is_sorted_until(v2.begin(), v2.end());

  if (it1 == v1.end()) {
    std::cout << "v1 is sorted" << std::endl;
  } else {
    std::cout << "v1 is not sorted up to " << *it1 << std::endl;
  }

  if (it2 == v2.end()) {
    std::cout << "v2 is sorted" << std::endl;
  } else {
    std::cout << "v2 is not sorted up to " << *it2 << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::is_sorted_until() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz. Ardından, std::is_sorted_until() işlevini kullanarak v1 ve v2 vektörlerinin sıralı olup olmadığını kontrol ediyoruz. Son olarak, her iki vektörün sıralı olup olmadığını ve sıralı olmayan son öğeyi yazdırıyoruz.

- Bu işlevin kullanımı, özellikle bir aralıktaki öğelerin belirli bir sıraya göre sıralanmış olduğu son öğeyi bulmak gerektiğinde oldukça faydalıdır.

### sort()

- std::sort() işlevi, bir aralıktaki öğeleri belirli bir sıraya göre sıralar. Bu işlev, C++'ın standart kitaplığındaki en önemli ve en sık kullanılan işlevlerden biridir.

- std::sort() işlevi, bir aralık için iki adet işaretçi parametresi alır. İşlev, belirtilen aralıktaki öğeleri sıralar. std::sort() işlevi, genellikle C++'ın standart sıralama algoritması olan quicksort algoritmasını kullanır. Bu algoritma, bir aralıktaki öğeleri hızlı bir şekilde sıralamak için etkilidir.

- İşte örnek bir kod parçası, std::sort() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {5, 2, 4, 6, 1, 3};

  std::sort(v.begin(), v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::sort() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::sort() işlevini kullanarak v vektöründeki öğeleri sıralıyoruz. Son olarak, sıralanmış öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğeleri belirli bir sıraya göre sıralamak gerektiğinde oldukça faydalıdır.

### partial_sort()
- std::partial_sort() işlevi, bir aralıktaki öğelerin bir kısmını belirli bir sıraya göre sıralar. Bu işlev, genellikle öncelikli olarak ilk N öğeyi sıralamak istediğiniz durumlarda kullanılır.

- std::partial_sort() işlevi, bir aralık için üç adet işaretçi parametresi alır. İlk parametre, sıralanacak aralığın başlangıcını işaret eder. İkinci parametre, sıralanacak aralığın sonunu işaret eder. Üçüncü parametre ise, sıralanacak öğelerin son sıralı konumunun işaretçisi olarak kullanılır. Bu işlevin çalışma mantığı, belirtilen son sıralı konumun sol tarafındaki öğeleri sıralamak ve son sıralı konumun sağ tarafındaki öğeleri sıralamamaktır.

- şte örnek bir kod parçası, std::partial_sort() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {5, 2, 4, 6, 1, 3};

  std::partial_sort(v.begin(), v.begin() + 3, v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::partial_sort() işlevinin kullanımını göstermektedir. İlk olarak, std::vector< int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::partial_sort() işlevini kullanarak v vektöründeki ilk üç öğeyi sıralıyoruz. Son olarak, sıralanmış öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğelerin bir kısmını belirli bir sıraya göre sıralamak istediğiniz durumlarda oldukça faydalıdır.

### partial_sort_copy

- std::partial_sort_copy() işlevi, bir aralıktaki öğelerin bir kısmını belirli bir sıraya göre sıralar ve sıralanmış öğeleri başka bir aralığa kopyalar. Bu işlev, std::partial_sort() işlevine benzer, ancak sıralanmış öğeleri yeni bir aralığa kopyalar.

- std::partial_sort_copy() işlevi, bir aralık için üç adet işaretçi parametresi ve başka bir aralık için iki adet işaretçi parametresi alır. İlk üç parametre, sıralanacak aralığın başlangıcını, sonunu ve son sıralı konumunun işaretçisini işaret eder. Dördüncü ve beşinci parametreler ise, sıralanmış öğelerin kopyalanacağı yeni aralığın başlangıcını ve sonunu işaret eder.

- İşte örnek bir kod parçası, std::partial_sort_copy() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {5, 2, 4, 6, 1, 3};
  std::vector<int> v2(3);

  std::partial_sort_copy(v.begin(), v.end(), v2.begin(), v2.end());

  for (auto it = v2.begin(); it != v2.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```
> Bu örnek kod, std::partial_sort_copy() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde v isimli bir vektör oluşturuyoruz. Ardından, std::vector int  türünde v2 isimli bir başka vektör oluşturuyoruz. Daha sonra, std::partial_sort_copy() işlevini kullanarak v vektöründeki öğelerin ilk üçünü sıralıyoruz ve v2 vektörüne kopyalıyoruz. Son olarak, sıralanmış öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğelerin bir kısmını belirli bir sıraya göre sıralamak ve sıralanmış öğeleri başka bir aralığa kopyalamak istediğiniz durumlarda oldukça faydalıdır.

### stable_sort()
  
- std::stable_sort() işlevi, bir aralıktaki öğeleri belirli bir sıraya göre sıralar. Bu işlev, std::sort() işlevine benzer, ancak sıralama işlemi sırasında öğelerin orijinal sıralama ilişkisi korunur. Bu nedenle, std::stable_sort() işlevi, öğelerin birbirine göre ilişkisini korumak istediğiniz durumlarda kullanılabilir.

- std::stable_sort() işlevi, bir aralık için iki adet işaretçi parametresi alır. İlk parametre, sıralanacak aralığın başlangıcını işaret eder. İkinci parametre, sıralanacak aralığın sonunu işaret eder. Bu işlevin çalışma mantığı, öğeleri sıralama işlemi sırasında orijinal sıralama ilişkisini koruyacak şekilde sıralamaktır.

- İşte örnek bir kod parçası, std::stable_sort() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {5, 2, 4, 6, 1, 3};

  std::stable_sort(v.begin(), v.end());

  for (auto it = v.begin(); it != v.end(); ++it) {
    std::cout << *it << " ";
  }

  return 0;
}

```

> Bu örnek kod, std::stable_sort() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Ardından, std::stable_sort() işlevini kullanarak v vektöründeki öğeleri sıralıyoruz. Son olarak, sıralanmış öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, öğelerin orijinal sıralama ilişkisini korumak istediğiniz durumlarda oldukça faydalıdır.

### nth_element

- std::nth_element() işlevi, bir aralıktaki öğelerin sadece belirli bir sıralamada olan n'inci öğesini bulmak için kullanılır. Bu işlev, özellikle büyük aralıkların sıralanması gerektiğinde ve sadece birkaç öğenin sıralanması gerektiğinde faydalıdır.

std::nth_element() işlevi, bir aralık için üç adet işaretçi parametresi alır. İlk parametre, sıralanacak aralığın başlangıcını işaret eder. İkinci parametre, sıralanacak aralığın sonunu işaret eder. Üçüncü parametre ise, sıralanacak öğelerin n'inci öğesi olacak şekilde belirtilir.

- İşte örnek bir kod parçası, std::nth_element() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {5, 2, 4, 6, 1, 3};
  int n = 3;

  std::nth_element(v.begin(), v.begin() + n, v.end());

  std::cout << "The " << n << "th element is " << v[n] << std::endl;

  return 0;
}

```

> Bu örnek kod, std::nth_element() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz ve n değişkenine 3 değerini atıyoruz. Ardından, std::nth_element() işlevini kullanarak v vektöründeki öğelerin 3'üncü öğesini belirliyoruz. Son olarak, belirtilen öğeyi yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki öğelerin sadece belirli bir sıralamada olan n'inci öğesini bulmak istediğiniz durumlarda oldukça faydalıdır.

### lower_bound()

- std::lower_bound() işlevi, bir aralıkta belirli bir değere veya daha büyük ilk değere sahip olan ilk öğenin konumunu (iterator'ünü) döndürür. Bu işlev, özellikle sıralanmış bir aralıkta bir değerin veya belirli bir değerden büyük ilk öğenin konumunu bulmak için kullanılır.

- std::lower_bound() işlevi, bir aralık için iki adet işaretçi parametresi ve bir değer parametresi alır. İlk parametre, aralığın başlangıcını işaret eder. İkinci parametre, aralığın sonunu işaret eder. Üçüncü parametre ise, aralıkta aranan değerdir.

- İşte örnek bir kod parçası, std::lower_bound() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6};
  int x = 4;

  auto it = std::lower_bound(v.begin(), v.end(), x);

  if (it != v.end()) {
    std::cout << "The first element >= " << x << " is at position " << (it - v.begin()) << std::endl;
  } else {
    std::cout << "No element found" << std::endl;
  }

  return 0;
}

```
> Bu örnek kod, std::lower_bound() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz ve x değişkenine 4 değerini atıyoruz. Ardından, std::lower_bound() işlevini kullanarak v vektöründe x değerinden büyük veya eşit ilk öğenin konumunu belirliyoruz. Son olarak, bu konumu yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıkta belirli bir değere veya daha büyük ilk değere sahip olan ilk öğenin konumunu (iterator'ünü) bulmak istediğiniz durumlarda oldukça faydalıdır.

### upper_bound
- std::upper_bound() işlevi, bir aralıkta belirli bir değerden büyük ilk öğenin konumunu (iterator'ünü) döndürür. Bu işlev, özellikle sıralanmış bir aralıkta bir değerden büyük ilk öğenin konumunu bulmak için kullanılır.

- std::upper_bound() işlevi, bir aralık için iki adet işaretçi parametresi ve bir değer parametresi alır. İlk parametre, aralığın başlangıcını işaret eder. İkinci parametre, aralığın sonunu işaret eder. Üçüncü parametre ise, aralıkta aranan değerdir.

- İşte örnek bir kod parçası, std::upper_bound() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6};
  int x = 4;

  auto it = std::upper_bound(v.begin(), v.end(), x);

  if (it != v.end()) {
    std::cout << "The first element > " << x << " is at position " << (it - v.begin()) << std::endl;
  } else {
    std::cout << "No element found" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::upper_bound() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz ve x değişkenine 4 değerini atıyoruz. Ardından, std::upper_bound() işlevini kullanarak v vektöründe x değerinden büyük ilk öğenin konumunu belirliyoruz. Son olarak, bu konumu yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıkta belirli bir değerden büyük ilk öğenin konumunu (iterator'ünü) bulmak istediğiniz durumlarda oldukça faydalıdır.

### equal_range

- std::binary_search() işlevi, sıralı bir aralıkta belirli bir değerin olup olmadığını kontrol eder. Eğer aralıkta değer varsa, true değerini döndürür; yoksa false değerini döndürür.

- std::binary_search() işlevi, bir aralık için iki adet işaretçi parametresi ve bir değer parametresi alır. İlk parametre, aralığın başlangıcını işaret eder. İkinci parametre, aralığın sonunu işaret eder. Üçüncü parametre ise, aralıkta aranan değerdir.

- İşte örnek bir kod parçası, std::binary_search() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {1, 2, 3, 4, 5, 6};
  int x = 4;

  if (std::binary_search(v.begin(), v.end(), x)) {
    std::cout << "The value " << x << " exists in the vector" << std::endl;
  } else {
    std::cout << "The value " << x << " does not exist in the vector" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::binary_search() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz ve x değişkenine 4 değerini atıyoruz. Ardından, std::binary_search() işlevini kullanarak v vektöründe x değerinin olup olmadığını kontrol ediyoruz. Son olarak, sonucu yazdırıyoruz.

- Bu işlevin kullanımı, sıralı bir aralıkta belirli bir değerin olup olmadığını kontrol etmek istediğiniz durumlarda oldukça faydalıdır.

### merge

- std::merge() işlevi, iki sıralı aralığı birleştirerek yeni bir sıralı aralık oluşturur. Birleştirme, iki aralıktaki tüm öğeleri sıralı bir şekilde birleştirir ve sonuç olarak yeni bir aralık oluşturur.

- std::merge() işlevi, üç adet işaretçi parametresi alır. İlk iki parametre, birleştirilecek iki sıralı aralığın başlangıç ve sonunu gösterir. Üçüncü parametre ise, birleştirilmiş aralığın başlangıcını gösterir. İşlev, birleştirilen aralığı tamamen sıralar, bu nedenle birleştirme işlemi öncesinde her iki aralık da sıralanmış olmalıdır.

- İşte örnek bir kod parçası, std::merge() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 3, 5, 7};
  std::vector<int> v2 {2, 4, 6, 8, 10};

  std::vector<int> v3(v1.size() + v2.size());

  std::merge(v1.begin(), v1.end(), v2.begin(), v2.end(), v3.begin());

  for (auto i : v3) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::merge() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve bu vektörleri sıralı hale getiriyoruz. Daha sonra, birleştirilmiş aralığı depolamak için yeni bir vektör oluşturuyoruz. std::merge() işlevini kullanarak v1 ve v2 vektörlerini birleştiriyoruz ve sonucu v3 vektörüne kaydediyoruz. Son olarak, v3 vektöründeki tüm öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, iki sıralı aralığı birleştirmek ve yeni bir sıralı aralık oluşturmak istediğiniz durumlarda oldukça faydalıdır.

### inplace_merge

- std::inplace_merge() işlevi, bir sıralı aralıktaki iki sıralı alt aralığı birleştirerek mevcut aralığı sıralı hale getirir. Bu işlev, özellikle sıralı bir aralıkta iki alt aralığı birleştirmek ve sonucu mevcut aralığa kaydetmek istediğiniz durumlarda kullanışlıdır.

- std::inplace_merge() işlevi, üç adet işaretçi parametresi alır. İlk iki parametre, birleştirilecek iki sıralı alt aralığın başlangıç ve sonunu gösterir. Üçüncü parametre ise, birleştirilen aralığın sonunu gösterir. İşlev, belirtilen iki alt aralığı birleştirir ve sonucunu, mevcut aralığın belirtilen sonu (üçüncü parametre) ile sınırlandırılmış bölgesine kaydeder.

- İşte örnek bir kod parçası, std::inplace_merge() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  auto mid = v.begin() + 5;

  std::inplace_merge(v.begin(), mid, v.end());

  for (auto i : v) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::inplace_merge() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz ve bu vektörü yazdırıyoruz. Daha sonra, mid adlı bir işaretçi oluşturuyoruz ve bu işaretçi, vektörün 5. öğesini işaret eder. std::inplace_merge() işlevini kullanarak, v vektöründe ilk 5 öğeyi ve sonraki öğeleri birleştiriyoruz. Son olarak, v vektöründeki tüm öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, bir sıralı aralıktaki iki alt aralığı birleştirmek ve sonucu mevcut aralığa kaydetmek istediğiniz durumlarda oldukça faydalıdır.

### includes()

- std::includes() işlevi, birinci sıralı aralığın ikinci sıralı aralığı içerip içermediğini kontrol eder. İkinci sıralı aralık, birinci sıralı aralığın bir alt kümesi olabilir veya olmayabilir.

- std::includes() işlevi, dört adet işaretçi parametresi alır. İlk iki parametre, birinci sıralı aralığın başlangıcını ve sonunu gösterir. Üçüncü ve dördüncü parametreler, ikinci sıralı aralığın başlangıcını ve sonunu gösterir. İşlev, ikinci sıralı aralığın birinci sıralı aralığı içerip içermediğini kontrol eder ve sonuç olarak true veya false değeri döndürür.

- İşte örnek bir kod parçası, std::includes() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5, 6};
  std::vector<int> v2 {3, 4, 5};

  if (std::includes(v1.begin(), v1.end(), v2.begin(), v2.end())) {
    std::cout << "The second vector is a subset of the first vector" << std::endl;
  } else {
    std::cout << "The second vector is not a subset of the first vector" << std::endl;
  }

  return 0;
}

```

> Bu örnek kod, std::includes() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz. Ardından, std::includes() işlevini kullanarak, v2 vektörünün v1 vektörünün bir alt kümesi olup olmadığını kontrol ediyoruz. Son olarak, sonucu yazdırıyoruz.

- Bu işlevin kullanımı, birinci sıralı aralığın ikinci sıralı aralığı içerip içermediğini kontrol etmek istediğiniz durumlarda oldukça faydalıdır.

### set_difference()

- std::set_difference() işlevi, iki sıralı aralık arasındaki farkı hesaplar ve sonucu yeni bir sıralı aralıkta depolar. İlk sıralı aralıktaki öğelerden, ikinci sıralı aralıktaki öğeleri çıkararak yeni bir sıralı aralık oluşturur.

- std::set_difference() işlevi, dört adet işaretçi parametresi alır. İlk iki parametre, birinci sıralı aralığın başlangıcını ve sonunu gösterir. Üçüncü ve dördüncü parametreler, ikinci sıralı aralığın başlangıcını ve sonunu gösterir. İşlev, ilk sıralı aralıktan ikinci sıralı aralıkta olmayan öğeleri yeni bir aralıkta depolar ve sonuc olarak bu yeni aralığı döndürür.

- İşte örnek bir kod parçası, std::set_difference() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {3, 4, 5, 6, 7};
  std::vector<int> v3(v1.size() + v2.size());

  std::set_difference(v1.begin(), v1.end(), v2.begin(), v2.end(), v3.begin());

  for (auto i : v3) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```

> Bu örnek kod, std::set_difference() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve bu vektörleri sıralı hale getiriyoruz. Daha sonra, v3 adlı yeni bir vektör oluşturuyoruz ve std::set_difference() işlevini kullanarak v1 vektöründeki öğelerden v2 vektöründeki öğeleri çıkararak yeni bir vektör oluşturuyoruz. Son olarak, bu yeni vektördeki tüm öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, iki sıralı aralık arasındaki farkı hesaplamak ve sonucu yeni bir sıralı aralıkta depolamak istediğiniz durumlarda oldukça faydalıdır.

### set_intersection()

- std::set_intersection() işlevi, iki sıralı aralık arasındaki kesişimi hesaplar ve sonucu yeni bir sıralı aralıkta depolar. Yani, iki sıralı aralıkta ortak olan öğelerden yeni bir aralık oluşturur.

- std::set_intersection() işlevi, dört adet işaretçi parametresi alır. İlk iki parametre, birinci sıralı aralığın başlangıcını ve sonunu gösterir. Üçüncü ve dördüncü parametreler, ikinci sıralı aralığın başlangıcını ve sonunu gösterir. İşlev, iki sıralı aralıkta ortak olan öğeleri yeni bir aralıkta depolar ve sonuc olarak bu yeni aralığı döndürür.

- İşte örnek bir kod parçası, std::set_intersection() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {3, 4, 5, 6, 7};
  std::vector<int> v3(std::min(v1.size(), v2.size()));

  auto it = std::set_intersection(v1.begin(), v1.end(), v2.begin(), v2.end(), v3.begin());

  for (auto i = v3.begin(); i != it; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::set_intersection() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve bu vektörleri sıralı hale getiriyoruz. Daha sonra, std::min() işlevini kullanarak v1 ve v2 vektörlerinin boyutlarından daha küçük olan bir boyutta v3 adlı yeni bir vektör oluşturuyoruz. std::set_intersection() işlevini kullanarak, v1 ve v2 vektörlerindeki ortak öğeleri v3 vektöründe saklıyoruz. Son olarak, v3 vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, iki sıralı aralık arasındaki kesişimi hesaplamak ve sonucu yeni bir sıralı aralıkta depolamak istediğiniz durumlarda oldukça faydalıdır.

### set_symmetric_difference()

- std::set_symmetric_difference() işlevi, iki sıralı aralık arasındaki simetrik farkı hesaplar ve sonucu yeni bir sıralı aralıkta depolar. İki sıralı aralıkta birinde olup diğerinde olmayan öğelerden yeni bir aralık oluşturur.

- std::set_symmetric_difference() işlevi, dört adet işaretçi parametresi alır. İlk iki parametre, birinci sıralı aralığın başlangıcını ve sonunu gösterir. Üçüncü ve dördüncü parametreler, ikinci sıralı aralığın başlangıcını ve sonunu gösterir. İşlev, iki sıralı aralıkta birinde olup diğerinde olmayan öğeleri yeni bir aralıkta depolar ve sonuc olarak bu yeni aralığı döndürür.

- İşte örnek bir kod parçası, std::set_symmetric_difference() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {3, 4, 5, 6, 7};
  std::vector<int> v3(v1.size() + v2.size());

  auto it = std::set_symmetric_difference(v1.begin(), v1.end(), v2.begin(), v2.end(), v3.begin());

  for (auto i = v3.begin(); i != it; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::set_symmetric_difference() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve bu vektörleri sıralı hale getiriyoruz. Daha sonra, v1 ve v2 vektörlerindeki öğelerden birinde olup diğerinde olmayan öğeleri std::set_symmetric_difference() işlevini kullanarak v3 adlı yeni bir vektörde saklıyoruz. Son olarak, v3 vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, iki sıralı aralık arasındaki simetrik farkı hesaplamak ve sonucu yeni bir sıralı aralıkta depolamak istediğiniz durumlarda oldukça faydalıdır.

### set_union()

- std::set_union() işlevi, iki sıralı aralık arasındaki birleşimi hesaplar ve sonucu yeni bir sıralı aralıkta depolar. İki sıralı aralıktaki öğelerin tümü yeni bir aralıkta birleştirilir.

- std::set_union() işlevi, dört adet işaretçi parametresi alır. İlk iki parametre, birinci sıralı aralığın başlangıcını ve sonunu gösterir. Üçüncü ve dördüncü parametreler, ikinci sıralı aralığın başlangıcını ve sonunu gösterir. İşlev, iki sıralı aralıktaki öğelerin tümünü yeni bir aralıkta birleştirir ve sonuc olarak bu yeni aralığı döndürür.

- İşte örnek bir kod parçası, std::set_union() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {3, 4, 5, 6, 7};
  std::vector<int> v3(v1.size() + v2.size());

  auto it = std::set_union(v1.begin(), v1.end(), v2.begin(), v2.end(), v3.begin());

  for (auto i = v3.begin(); i != it; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::set_union() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve bu vektörleri sıralı hale getiriyoruz. Daha sonra, v1 ve v2 vektörlerindeki tüm öğeleri std::set_union() işlevini kullanarak v3 adlı yeni bir vektörde birleştiriyoruz. Son olarak, v3 vektöründeki öğeleri yazdırıyoruz.

- Bu işlevin kullanımı, iki sıralı aralık arasındaki birleşimi hesaplamak ve sonucu yeni bir sıralı aralıkta depolamak istediğiniz durumlarda oldukça faydalıdır.

### is_heap()

- std::is_heap() işlevi, verilen aralığın bir maksimum yığın mı olduğunu kontrol eder. Bir maksimum yığın, herhangi bir düğümün çocuklarından daha büyük veya eşit olduğu bir ağaçtır.

- std::is_heap() işlevi, iki adet işaretçi parametresi alır. İlk parametre, aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. İşlev, verilen aralığın bir maksimum yığın olup olmadığını kontrol eder ve sonucu bir bool değer olarak döndürür.

- İşte örnek bir kod parçası, std::is_heap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {1, 3, 2, 4, 5};

  std::cout << std::boolalpha << std::is_heap(v1.begin(), v1.end()) << std::endl;
  std::cout << std::boolalpha << std::is_heap(v2.begin(), v2.end()) << std::endl;

  return 0;
}

```
> Bu örnek kod, std::is_heap() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve v1 vektörü bir maksimum yığın iken v2 vektörü bir maksimum yığın değildir. Daha sonra, std::is_heap() işlevini kullanarak v1 ve v2 vektörlerinin maksimum yığın olup olmadığını kontrol ediyoruz ve sonucu ekrana yazdırıyoruz.

- Bu işlevin kullanımı, verilen bir aralığın maksimum yığın olup olmadığını kontrol etmek istediğiniz durumlarda oldukça faydalıdır.

### is_heap_until()

- std::is_heap_until() işlevi, verilen aralığın maksimum yığın özelliği gösteren bölgenin sonunu döndürür. Maksimum yığın, herhangi bir düğümün çocuklarından daha büyük veya eşit olduğu bir ağaçtır.

- std::is_heap_until() işlevi, iki adet işaretçi parametresi alır. İlk parametre, aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. İşlev, verilen aralığın maksimum yığın özelliği gösteren bölgenin sonunu döndürür.

- İşte örnek bir kod parçası, std::is_heap_until() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {1, 3, 2, 4, 5};

  auto it1 = std::is_heap_until(v1.begin(), v1.end());
  auto it2 = std::is_heap_until(v2.begin(), v2.end());

  std::cout << "v1: ";
  for (auto i = v1.begin(); i != it1; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  std::cout << "v2: ";
  for (auto i = v2.begin(); i != it2; ++i) {
    std::cout << *i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::is_heap_until() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1 ve v2 isimli iki vektör oluşturuyoruz ve v1 vektörü bir maksimum yığın iken v2 vektörü bir maksimum yığın değildir. Daha sonra, std::is_heap_until() işlevini kullanarak v1 ve v2 vektörlerinin maksimum yığın özelliği gösteren bölgenin sonunu buluyoruz ve sonucu ekrana yazdırıyoruz.

- Bu işlevin kullanımı, verilen bir aralığın maksimum yığın özelliği gösteren bölgesinin sonunu bulmak istediğiniz durumlarda oldukça faydalıdır.

### make_heap()

- std::make_heap() işlevi, verilen bir aralığı maksimum yığın haline getirir. Maksimum yığın, herhangi bir düğümün çocuklarından daha büyük veya eşit olduğu bir ağaçtır.

- std::make_heap() işlevi, iki adet işaretçi parametresi alır. İlk parametre, aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. İşlev, verilen aralığı maksimum yığın haline getirir.

- İşte örnek bir kod parçası, std::make_heap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  std::make_heap(v.begin(), v.end());

  std::cout << "v: ";
  for (auto i : v) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::make_heap() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::make_heap() işlevini kullanarak v vektörünü maksimum yığın haline getiriyoruz ve sonucu ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığı maksimum yığın haline getirmek istediğiniz durumlarda oldukça faydalıdır.

### push_heap()

- std::push_heap() işlevi, verilen bir aralığın sonuna yeni bir eleman ekleyerek maksimum yığın özelliğini yeniden oluşturur. Maksimum yığın, herhangi bir düğümün çocuklarından daha büyük veya eşit olduğu bir ağaçtır.

- std::push_heap() işlevi, iki adet işaretçi parametresi alır. İlk parametre, aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. İşlev, yeni eklenen elemanı yığın haline getirir.

- İşte örnek bir kod parçası, std::push_heap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  v.push_back(7);
  std::push_heap(v.begin(), v.end());

  std::cout << "v: ";
  for (auto i : v) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```

> Bu örnek kod, std::push_heap() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, v vektörüne push_back() işlevi ile yeni bir eleman ekliyoruz ve std::push_heap() işlevini kullanarak v vektörünü maksimum yığın haline getiriyoruz. Son olarak, v vektörünü ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığa yeni bir eleman ekledikten sonra maksimum yığın özelliğini yeniden oluşturmak istediğiniz durumlarda oldukça faydalıdır.

### pop_heap()

- std::pop_heap() işlevi, maksimum yığın özelliğine sahip bir aralığın en büyük elemanını, aralığın sonundan çıkartır. Daha sonra, en büyük eleman aralığın sonuna yerleştirilir. Maksimum yığın, herhangi bir düğümün çocuklarından daha büyük veya eşit olduğu bir ağaçtır.

- std::pop_heap() işlevi, iki adet işaretçi parametresi alır. İlk parametre, aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. İşlev, en büyük elemanı aralığın sonuna yerleştirir.

- İşte örnek bir kod parçası, std::pop_heap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  std::pop_heap(v.begin(), v.end());
  int max = v.back();
  v.pop_back();

  std::cout << "max: " << max << std::endl;

  std::cout << "v: ";
  for (auto i : v) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::pop_heap() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::pop_heap() işlevini kullanarak v vektörünün en büyük elemanını aralığın sonuna yerleştiriyoruz. Daha sonra, en büyük elemanı back() işlevi ile alıyoruz ve aralıktan çıkartıyoruz. Son olarak, en büyük elemanı ve aralığı ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir maksimum yığın özelliğine sahip bir aralıktan en büyük elemanı çıkartmak istediğiniz durumlarda oldukça faydalıdır.

### sort_heap()

- std::sort_heap() işlevi, bir aralığın maksimum yığın özelliğine sahip olduğu varsayımını kullanarak aralığı sıralar. Maksimum yığın, herhangi bir düğümün çocuklarından daha büyük veya eşit olduğu bir ağaçtır.

- std::sort_heap() işlevi, iki adet işaretçi parametresi alır. İlk parametre, aralığın başlangıcını gösteren bir işaretçidir. İkinci parametre, aralığın sonunu gösteren bir işaretçidir. İşlev, aralığı sıralar.

- İşte örnek bir kod parçası, std::sort_heap() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  std::make_heap(v.begin(), v.end());
  std::sort_heap(v.begin(), v.end());

  std::cout << "v: ";
  for (auto i : v) {
    std::cout << i << " ";
  }
  std::cout << std::endl;

  return 0;
}

```
> Bu örnek kod, std::sort_heap() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::make_heap() işlevini kullanarak v vektörünü maksimum yığın haline getiriyoruz. Son olarak, std::sort_heap() işlevini kullanarak v vektörünü sıralıyoruz ve aralığı ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralığın maksimum yığın özelliğine sahip olduğu durumlarda aralığı sıralamak istediğiniz durumlarda oldukça faydalıdır.

### max()

- std::max() işlevi, verilen iki argüman arasındaki en büyük değeri döndürür. İki argüman aynı türden olmalıdır ve argümanlar karşılaştırılabilir olmalıdır (yani, < ve > operatörleri kullanılabilir).

- std::max() işlevi, iki adet argüman alır. İlk argüman, karşılaştırılacak ilk değerdir. İkinci argüman, karşılaştırılacak ikinci değerdir. İşlev, bu iki değer arasındaki en büyük değeri döndürür.

- İşte örnek bir kod parçası, std::max() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>

int main() {
  int x = 10;
  int y = 20;

  int max_value = std::max(x, y);

  std::cout << "max value: " << max_value << std::endl;

  return 0;
}

```

> Bu örnek kod, std::max() işlevinin kullanımını göstermektedir. İlk olarak, x ve y isimli iki tamsayı değişkeni oluşturuyoruz. Daha sonra, std::max() işlevini kullanarak x ve y arasındaki en büyük değeri hesaplıyoruz ve max_value isimli bir değişkende saklıyoruz. Son olarak, max_value değişkenini ekrana yazdırıyoruz.

Bu işlevin kullanımı, iki argüman arasındaki en büyük değeri bulmak istediğiniz durumlarda oldukça faydalıdır.

### max_element()

- std::max_element() işlevi, bir aralıktaki en büyük değeri bulmak için kullanılır. İşlev, iki adet işaretçi parametresi alır: aralığın başlangıcını ve sonunu gösteren işaretçiler. Aralıktaki en büyük değeri içeren işaretçi, işlev tarafından geri döndürülür.

- İşlev, aralıkta bulunan elemanları karşılaştırmak için < operatörünü kullanır. Karşılaştırma işlemi, elemanların türündeki < operatörüne göre yapılır. Bu nedenle, aralıktaki elemanların bu operatöre sahip olması gerekmektedir.

- İşte örnek bir kod parçası, std::max_element() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  auto max_element_ptr = std::max_element(v.begin(), v.end());

  std::cout << "max element: " << *max_element_ptr << std::endl;

  return 0;
}

```

> Bu örnek kod, std::max_element() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::max_element() işlevini kullanarak v vektöründeki en büyük elemanı içeren bir işaretçi alıyoruz. Son olarak, en büyük elemanı ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki en büyük değeri bulmak istediğiniz durumlarda oldukça faydalıdır.

### min()

- std::min() işlevi, verilen iki argüman arasındaki en küçük değeri döndürür. İki argüman aynı türden olmalıdır ve argümanlar karşılaştırılabilir olmalıdır (yani, < ve > operatörleri kullanılabilir).

- std::min() işlevi, iki adet argüman alır. İlk argüman, karşılaştırılacak ilk değerdir. İkinci argüman, karşılaştırılacak ikinci değerdir. İşlev, bu iki değer arasındaki en küçük değeri döndürür.

- İşte örnek bir kod parçası, std::min() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>

int main() {
  int x = 10;
  int y = 20;

  int min_value = std::min(x, y);

  std::cout << "min value: " << min_value << std::endl;

  return 0;
}

```
> Bu örnek kod, std::min() işlevinin kullanımını göstermektedir. İlk olarak, x ve y isimli iki tamsayı değişkeni oluşturuyoruz. Daha sonra, std::min() işlevini kullanarak x ve y arasındaki en küçük değeri hesaplıyoruz ve min_value isimli bir değişkende saklıyoruz. Son olarak, min_value değişkenini ekrana yazdırıyoruz.

- Bu işlevin kullanımı, iki argüman arasındaki en küçük değeri bulmak istediğiniz durumlarda oldukça faydalıdır.

### min_element()

- std::min_element() işlevi, bir aralıktaki en küçük değeri bulmak için kullanılır. İşlev, iki adet işaretçi parametresi alır: aralığın başlangıcını ve sonunu gösteren işaretçiler. Aralıktaki en küçük değeri içeren işaretçi, işlev tarafından geri döndürülür.

- İşlev, aralıkta bulunan elemanları karşılaştırmak için < operatörünü kullanır. Karşılaştırma işlemi, elemanların türündeki < operatörüne göre yapılır. Bu nedenle, aralıktaki elemanların bu operatöre sahip olması gerekmektedir.

- İşte örnek bir kod parçası, std::min_element() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  auto min_element_ptr = std::min_element(v.begin(), v.end());

  std::cout << "min element: " << *min_element_ptr << std::endl;

  return 0;
}

```
> Bu örnek kod, std::min_element() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::min_element() işlevini kullanarak v vektöründeki en küçük elemanı içeren bir işaretçi alıyoruz. Son olarak, en küçük elemanı ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki en küçük değeri bulmak istediğiniz durumlarda oldukça faydalıdır.

### minmax()

- std::minmax() işlevi, bir aralıktaki en küçük ve en büyük değerleri bulmak için kullanılır. İşlev, iki adet işaretçi parametresi alır: aralığın başlangıcını ve sonunu gösteren işaretçiler. Aralıktaki en küçük ve en büyük değerleri içeren bir std::pair nesnesi, işlev tarafından geri döndürülür.

- İşlev, aralıkta bulunan elemanları karşılaştırmak için < operatörünü kullanır. Karşılaştırma işlemi, elemanların türündeki < operatörüne göre yapılır. Bu nedenle, aralıktaki elemanların bu operatöre sahip olması gerekmektedir.

- İşte örnek bir kod parçası, std::minmax() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  auto minmax_pair = std::minmax_element(v.begin(), v.end());

  std::cout << "min element: " << *minmax_pair.first << std::endl;
  std::cout << "max element: " << *minmax_pair.second << std::endl;

  return 0;
}

```
> Bu örnek kod, std::minmax() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::minmax_element() işlevini kullanarak v vektöründeki en küçük ve en büyük elemanları içeren bir std::pair nesnesi alıyoruz. Son olarak, en küçük ve en büyük elemanları ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki en küçük ve en büyük değerleri bulmak istediğiniz durumlarda oldukça faydalıdır.

### minmax_element()

- std::minmax_element() işlevi, bir aralıktaki en küçük ve en büyük değerleri bulmak için kullanılır. İşlev, iki adet işaretçi parametresi alır: aralığın başlangıcını ve sonunu gösteren işaretçiler. Aralıktaki en küçük ve en büyük değerleri içeren bir std::pair nesnesi, işlev tarafından geri döndürülür.

- İşlev, aralıkta bulunan elemanları karşılaştırmak için < operatörünü kullanır. Karşılaştırma işlemi, elemanların türündeki < operatörüne göre yapılır. Bu nedenle, aralıktaki elemanların bu operatöre sahip olması gerekmektedir.

- İşte örnek bir kod parçası, std::minmax_element() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v {3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5};

  auto minmax_element_pair = std::minmax_element(v.begin(), v.end());

  std::cout << "min element: " << *minmax_element_pair.first << std::endl;
  std::cout << "max element: " << *minmax_element_pair.second << std::endl;

  return 0;
}

```
> Bu örnek kod, std::minmax_element() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v isimli bir vektör oluşturuyoruz. Daha sonra, std::minmax_element() işlevini kullanarak v vektöründeki en küçük ve en büyük elemanları içeren bir std::pair nesnesi alıyoruz. Son olarak, en küçük ve en büyük elemanları ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir aralıktaki en küçük ve en büyük değerleri bulmak istediğiniz durumlarda oldukça faydalıdır.

### clamp()

- std::clamp() işlevi, bir değerin belirli bir aralıkta olmasını sağlamak için kullanılır. İşlev, üç adet parametre alır: değer, alt sınır ve üst sınır. Eğer değer alt sınırdan küçükse, alt sınır değeri döndürülür. Eğer değer üst sınırdan büyükse, üst sınır değeri döndürülür. Aksi takdirde, değer kendisi döndürülür.

- std::clamp() işlevi, std::min() ve std::max() işlevlerinin birleşimi olarak düşünülebilir. İşte örnek bir kod parçası, std::clamp() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>

int main() {
  int x = 5;

  // Clamping x to the range [1, 10]
  x = std::clamp(x, 1, 10);

  std::cout << "x: " << x << std::endl;

  return 0;
}

```

> Bu örnek kod, std::clamp() işlevinin kullanımını göstermektedir. İlk olarak, int türünde x isimli bir değişken oluşturuyoruz. Daha sonra, std::clamp() işlevini kullanarak x değerini 1 ile 10 arasında kalmak üzere kısıtlıyoruz. Son olarak, x değerini ekrana yazdırıyoruz.

- Bu işlevin kullanımı, bir değerin belirli bir aralıkta kalmasını sağlamak istediğiniz durumlarda oldukça faydalıdır.

### equal()

- std::equal() işlevi, iki aralıktaki elemanların eşit olup olmadığını kontrol etmek için kullanılır. İşlev, iki adet işaretçi parametresi alır: ilk aralığın başlangıcını ve sonunu gösteren işaretçiler ve ikinci aralığın başlangıcını gösteren bir işaretçi. Eğer iki aralıkta aynı elemanlar varsa, işlev true değerini döndürür. Aksi takdirde, false değerini döndürür.

- İşlev, aralıktaki elemanları karşılaştırmak için == operatörünü kullanır. Karşılaştırma işlemi, elemanların türündeki == operatörüne göre yapılır. Bu nedenle, aralıktaki elemanların bu operatöre sahip olması gerekmektedir.

- İşte örnek bir kod parçası, std::equal() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {1, 2, 3, 4, 5};
  std::vector<int> v3 {5, 4, 3, 2, 1};

  bool result1 = std::equal(v1.begin(), v1.end(), v2.begin());
  bool result2 = std::equal(v1.begin(), v1.end(), v3.begin());

  std::cout << "v1 and v2 are equal: " << result1 << std::endl;
  std::cout << "v1 and v3 are equal: " << result2 << std::endl;

  return 0;
}

```

> Bu örnek kod, std::equal() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1, v2 ve v3 isimli üç vektör oluşturuyoruz. Daha sonra, std::equal() işlevini kullanarak v1 ve v2 vektörleri ile v1 ve v3 vektörleri arasındaki eşitliği kontrol ediyoruz. Son olarak, bu eşitlikleri ekrana yazdırıyoruz.

- Bu işlevin kullanımı, iki aralık arasındaki eşitliği kontrol etmek istediğiniz durumlarda oldukça faydalıdır.

### lexicographical_compare()

- std::lexicographical_compare() işlevi, iki aralıktaki elemanların leksikografik olarak karşılaştırılmasını sağlar. İşlev, iki adet işaretçi parametresi alır: ilk aralığın başlangıcını ve sonunu gösteren işaretçiler ve ikinci aralığın başlangıcını gösteren bir işaretçi. İşlev, iki aralıktaki elemanları sırayla karşılaştırarak ilerler. Eğer ilk aralıktaki eleman, ikinci aralıktaki elemandan küçükse, işlev true değerini döndürür. Eğer ilk aralıktaki eleman, ikinci aralıktaki elemandan büyükse, işlev false değerini döndürür. Eğer iki eleman eşitse, işlev karşılaştırmaya devam eder. Eğer ilk aralıktaki elemanlar tamamen ikinci aralıktaki elemanlardan küçükse, işlev true değerini döndürür. Aksi takdirde, false değerini döndürür.

- İşte örnek bir kod parçası, std::lexicographical_compare() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {1, 2, 3, 4, 6};
  std::vector<int> v3 {1, 2, 3, 4, 4};

  bool result1 = std::lexicographical_compare(v1.begin(), v1.end(), v2.begin(), v2.end());
  bool result2 = std::lexicographical_compare(v1.begin(), v1.end(), v3.begin(), v3.end());

  std::cout << "v1 is less than v2: " << result1 << std::endl;
  std::cout << "v1 is less than v3: " << result2 << std::endl;

  return 0;
}

```
> Bu örnek kod, std::lexicographical_compare() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1, v2 ve v3 isimli üç vektör oluşturuyoruz. Daha sonra, std::lexicographical_compare() işlevini kullanarak v1 ve v2 vektörlerinin leksikografik olarak karşılaştırılması ile v1 ve v3 vektörleri arasındaki karşılaştırmanın sonuçlarını hesaplıyoruz. Son olarak, bu sonuçları ekrana yazdırıyoruz.

- Bu işlevin kullanımı, iki aralık arasındaki leksikografik sıralamayı karşılaştırmak istediğiniz durumlarda oldukça faydalıdır.

### lexicographical_compare_three_way()

- std::lexicographical_compare_three_way() işlevi, iki aralıktaki elemanların üçlü karşılaştırmasını yapar ve sonuç olarak std::strong_ordering türünden bir değer döndürür. İşlev, iki adet işaretçi parametresi alır: ilk aralığın başlangıcını ve sonunu gösteren işaretçiler ve ikinci aralığın başlangıcını gösteren bir işaretçi. İşlev, iki aralıktaki elemanları sırayla karşılaştırarak ilerler. İlk olarak, iki elemanın karşılaştırması yapılır. Eğer iki eleman eşitse, karşılaştırmaya devam edilir. Eğer ilk aralıktaki eleman, ikinci aralıktaki elemandan küçükse, işlev std::strong_ordering::less değerini döndürür. Eğer ilk aralıktaki eleman, ikinci aralıktaki elemandan büyükse, işlev std::strong_ordering::greater değerini döndürür. Eğer iki eleman eşitse, karşılaştırmaya devam edilir. Eğer ilk aralıktaki elemanlar tamamen ikinci aralıktaki elemanlardan küçükse, işlev std::strong_ordering::less değerini döndürür. Eğer ilk aralıktaki elemanlar tamamen ikinci aralıktaki elemanlardan büyükse, işlev std::strong_ordering::greater değerini döndürür. Eğer iki aralıkta elemanlar aynıysa, işlev std::strong_ordering::equal değerini döndürür.

- İşte örnek bir kod parçası, std::lexicographical_compare_three_way() işlevinin nasıl kullanılabileceğini gösteriyor:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
  std::vector<int> v1 {1, 2, 3, 4, 5};
  std::vector<int> v2 {1, 2, 3, 4, 6};
  std::vector<int> v3 {1, 2, 3, 4, 4};

  auto result1 = std::lexicographical_compare_three_way(v1.begin(), v1.end(), v2.begin(), v2.end());
  auto result2 = std::lexicographical_compare_three_way(v1.begin(), v1.end(), v3.begin(), v3.end());

  std::cout << "v1 is less than v2: " << (result1 == std::strong_ordering::less) << std::endl;
  std::cout << "v1 is less than v3: " << (result2 == std::strong_ordering::less) << std::endl;

  return 0;
}

```
> Bu örnek kod, std::lexicographical_compare_three_way() işlevinin kullanımını göstermektedir. İlk olarak, std::vector int  türünde v1, v2 ve v3 isimli üç vektör oluşturuy. Daha sonra, std::lexicographical_compare_three_way() işlevini kullanarak v1 ve v2 vektörlerinin üçlü karşılaştırmasını yaparak sonucu result1 değişkeninde saklıyoruz. Benzer şekilde, v1 ve v3 vektörleri arasındaki üçlü karşılaştırmanın sonucunu result2 değişkeninde saklıyoruz. Son olarak, bu sonuçları ekrana yazdırıyoruz. std::strong_ordering::less değeri, karşılaştırılan ilk aralığın elemanlarının ikinci aralıktakinin elemanlarından küçük olduğunu gösterir.

Bu işlevin kullanımı, iki aralık arasındaki leksikografik sıralamayı karşılaştırmak istediğiniz durumlarda oldukça faydalıdır. std::lexicographical_compare() işlevinden farklı olarak, std::lexicographical_compare_three_way() işlevi üçlü karşılaştırma yapar ve sonuç olarak std::strong_ordering türünden bir değer döndürür. Bu sayede, karşılaştırma sonucu ile ilgili daha fazla bilgi elde edilebilir.

### is_permutation()


- std::is_permutation() işlevi, iki aralıkta bulunan elemanların birbirlerinin permütasyonu olup olmadığını kontrol eder. Yani, her iki aralıkta da aynı elemanlar varsa ve sıraları da farklı olabilir, ancak her bir eleman yalnızca bir kez geçiyorsa, bu durumda iki aralık birbirinin permütasyonudur.

- İşlev, üç parametre alır: iki aralık ve bir karşılaştırma işlevi (opsiyonel). Karşılaştırma işlevi, iki elemanı karşılaştırmak için kullanılır. Varsayılan olarak, std::equal_to<> kullanılır.

- İşlev, bool türünden bir değer döndürür. Eğer iki aralık birbirinin permütasyonuysa true değerini, aksi takdirde false değerini döndürür.

- İşte örnek bir kullanımı:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
    std::vector<int> v1 = {1, 2, 3, 4, 5};
    std::vector<int> v2 = {3, 5, 1, 4, 2};
    std::vector<int> v3 = {1, 2, 3, 4, 4};

    bool result1 = std::is_permutation(v1.begin(), v1.end(), v2.begin());
    bool result2 = std::is_permutation(v1.begin(), v1.end(), v3.begin());

    std::cout << std::boolalpha;
    std::cout << "v1 is permutation of v2: " << result1 << '\n';
    std::cout << "v1 is permutation of v3: " << result2 << '\n';

    return 0;
}

```

> Bu örnek kodda, std::vector int  türünden v1, v2 ve v3 isimli üç farklı vektör oluşturulmuştur. Daha sonra, std::is_permutation() işlevi kullanılarak v1 ve v2 vektörleri arasında bir permütasyon olup olmadığı kontrol edilmiş ve sonuç result1 değişkeninde saklanmıştır. Benzer şekilde, v1 ve v3 vektörleri arasında bir permütasyon olup olmadığı kontrol edilerek sonuç result2 değişkeninde saklanmıştır.

- Son olarak, sonuçlar ekrana yazdırılmıştır. std::boolalpha manipülatörü kullanılarak true veya false değerleri yerine true veya false yazıları yazdırılmıştır.

### next_permutation()

- std::next_permutation() işlevi, bir aralıktaki elemanların permütasyonlarını bulmaya yarayan bir işlemdir. İlk çağrıda, işlev, aralıktaki elemanları küçükten büyüğe doğru sıralar. Daha sonra, her çağrıda bir sonraki permütasyonu bulur. Eğer aralıktaki son permütasyona gelinirse, işlev false değerini döndürür. Bu durumda, aralıktaki elemanlar tekrar ilk permütasyona döndürülür.

- İşlev, iki parametre alır: başlangıç ve bitiş iterator'ları. İkinci parametre opsiyoneldir ve aralık sonunda bulunan "bir sonraki" permütasyonun bulunup bulunmadığını gösteren bir bool değeri döndürür. Varsayılan olarak, bu parametre true olarak ayarlanmıştır.

- İşte örnek bir kullanımı:

```CPP

#include <iostream>
#include <algorithm>
#include <vector>

int main() {
    std::vector<int> v = {1, 2, 3};

    do {
        for (auto i : v) {
            std::cout << i << ' ';
        }
        std::cout << '\n';
    } while (std::next_permutation(v.begin(), v.end()));

    return 0;
}

```

> Bu örnek kodda, std::vector int  türünden v isimli bir vektör oluşturulmuştur. Daha sonra, do-while döngüsü kullanılarak, std::next_permutation() işlevi kullanılarak tüm permütasyonlar elde edilir ve ekrana yazdırılır.

- İlk çağrıda, v vektöründeki elemanlar küçükten büyüğe doğru sıralanır. Daha sonra, do-while döngüsü kullanılarak, std::next_permutation() işlevi kullanılarak tüm permütasyonlar elde edilir ve ekrana yazdırılır. Son olarak, std::next_permutation() işlevi false değerini döndürdüğünde, döngü sonlanır.

### prev_permutation()

- std::prev_permutation() işlevi, std::next_permutation() işlevinin tam tersi olan bir işlemdir. Bu işlev, bir aralıktaki elemanların permütasyonlarını bulmaya yarar. İlk çağrıda, işlev, aralıktaki elemanları büyükten küçüğe doğru sıralar. Daha sonra, her çağrıda bir önceki permütasyonu bulur. Eğer aralıktaki ilk permütasyona gelinirse, işlev false değerini döndürür. Bu durumda, aralıktaki elemanlar tekrar son permütasyona döndürülür.

- İşlev, iki parametre alır: başlangıç ve bitiş iterator'ları. İkinci parametre opsiyoneldir ve aralık sonunda bulunan "bir önceki" permütasyonun bulunup bulunmadığını gösteren bir bool değeri döndürür. Varsayılan olarak, bu parametre true olarak ayarlanmıştır.

- İşte örnek bir kullanımı:

```CPP
#include <iostream>
#include <algorithm>
#include <vector>

int main() {
    std::vector<int> v = {3, 2, 1};

    do {
        for (auto i : v) {
            std::cout << i << ' ';
        }
        std::cout << '\n';
    } while (std::prev_permutation(v.begin(), v.end()));

    return 0;
}

```

> Bu örnek kodda, std::vector<int> türünden v isimli bir vektör oluşturulmuştur. Daha sonra, do-while döngüsü kullanılarak, std::prev_permutation() işlevi kullanılarak tüm permütasyonlar elde edilir ve ekrana yazdırılır.

- İlk çağrıda, v vektöründeki elemanlar büyükten küçüğe doğru sıralanır. Daha sonra, do-while döngüsü kullanılarak, std::prev_permutation() işlevi kullanılarak tüm permütasyonlar elde edilir ve ekrana yazdırılır. Son olarak, std::prev_permutation() işlevi false değerini döndürdüğünde, döngü sonlanır.














