# git-github-cheatsheet

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


- Git projesi oluşturmak.

```console
$ cd git
$ git init
```

- Proje dosyalarını listelemek (dizin içerisinde gizli bir .git dosyası oluşur.).

```console
$ ls -a
```

- Dizin içerisindeki dosyaları geçiş bölgesine taşımak. 
- (.) ifadesi dizin içerisindeki tüm dosyaları ifade eder.

```console
$ git add .
```


- git üzerinde bir kopya oluşturmak (commit).

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

