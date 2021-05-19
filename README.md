# git-github-cheatsheet


## GIT

- Git'e kendimizi tanıtmak.

```console
$ git config --global user.name "Mustafa Dikyar"
$ git config --global user.email "iammustafadikyar@gmail.com"
```


- Yapılandırmamızı kontrol etmek.

```console
$ git config --global user.name
$ git config --global user.email
```


- Bulunduğumuz dizinin yolu almak.

```console
$ pwd
```


- Bulunduğumuz dizin içerisindeki dosyaları listelemek.

```console
$ ls
```


- Farklı bir dizine (Change Directory) geçmek.
```console
$ cd C:
```

- Bir önceki dizine geçmek.

```console
$ cd ..
```

- Terminali temizlemek (Kısayol : Ctrl + L).

```console
$ clear
```


- Çalışma dizini (Working Directory) içerisine git projesi oluşturmak.

```console
$ cd git
$ git init
```

- Çalışma dizini içerisindeki proje dosyalarını listelemek (dizin içerisinde gizli bir .git dosyası oluşur.).

```console
$ ls -a
```

- Çalışma dizini içerisindeki dosyaları geçiş bölgesine (Staging Area) taşımak. 
- (.) ifadesi dizin içerisindeki tüm dosyaları ifade eder.

```console
$ git add .
```


- git deposu (repository) üzerinde bir kopya oluşturmak (commit).

```console
$ git commit -m "first commit"
```


- Log kayıtlarını görmek.

```console
$ git log
```


- Proje üzerindeki değişiklikleri görmek.
- Eğer bir değişiklik yapıldıysa kırmızı bir font ile belirtilmiş 'modified:' ön ekiyle geçiş bölgesine taşınabilecek dosyaların bir listesini sunar.

```console
$ git status
```


- Yapılan değişiklikleri önce geçiş alanına sonra da bir kopyasını git üzerine taşımak.

```console
$ git add start.cs
$ git commit -m "Has been a changed."
```


- Yapılan değişiklikleri incelemek.
- Eklenen satırlar (+) ve yeşil bir font ile çıkarılan satırlar (-) ve kırmızı bir font ile satır satır listelenir.

```console
$ git diff
```

** Silme, isim değiştirme, dizin değişikliği gibi işlemler komut satırı ile yapılabildiği gibi manuel olarak ta yapılabilir. 

- Dosyaları silmek.
- Manuel olarak silip sonrasında commit yaparak ta silme işlemi yapılabilir.

```console
$ git rm start.dart
$ git commit -m "start.dart is deleted."
```


- Klasör silmek

```console
$ git rm -r deleted/
$ git commit -m "'deleted' folder is deleted."
```


- Dosyayı yeniden adlandırmak.

```console
$ git mv start.cs updated.dart
$ git commit -m "Name change 'start.cs' -> 'updated.dart'"
```


- Dosyayı farklı bir dizine taşımak

```console
$ git mv updated.dart folder-to-move/
$ git commit -m "updated.dart has been moved."
```


- Çalışma alanında yapılan işlemleri geri almak.
- Birden fazla dosya üzerinde işlem yapılabilir.

```console
$ git checkout -- updated.dart
```


- Geçiş bölgesinde yapılan işlemleri geri almak.

```console
$ git restore --staged folder-to-move/updated.dart
$ git checkout -- folder-to-move/updated.dart
```


- Versiyon değiştirmek
- log kayıtlarını getirerek ilgili id'ye erişilebilir. (ee09f5bfd7d76e2235f4e3bbc79c6f5d1b676a2e)

```console
$ git log
$ git checkout ee09f5bfd7d76e2235f4e3bbc79c6f5d1b676a2e -- .
$ git commit -m "All changes have been reverted."
```


- GITHUB ile devam edilecek.

