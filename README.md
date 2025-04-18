# Libft

Libft, C programlama dili ile yazılmış, C'nin standart kütüphane fonksiyonlarının yeniden inşa edildiği kişisel bir kütüphane projesidir. Bu proje, temel programlama yeteneklerini pekiştirmek, bellek yönetimi ve düşük seviye programlama konularında derinleşmek amacıyla 42 okullarında zorunlu olarak yapılır.

## 🚀 Özellikler

- Standart C fonksiyonlarının yeniden yazımı:
  - `strlen`, `strcpy`, `memset`, `memcmp`, `atoi`, `calloc` vs.
- String ve bellek işlemleri
- Karakter kontrol fonksiyonları (`isalpha`, `isdigit`, `toupper`, `tolower` vb.)
- Linked list (bağlı liste) veri yapısı ve ilgili yardımcı fonksiyonlar

## 📁 Proje Yapısı

Kategori | Fonksiyonlar
---------|--------------
Karakter Kontrolü | [`ft_isalpha`](https://github.com/rumeysaispay/Libft/blob/main/ft_isalpha.c), [`ft_isdigit`](https://github.com/rumeysaispay/Libft/blob/main/ft_isdigit.c), [`ft_isalnum`](https://github.com/rumeysaispay/Libft/blob/main/ft_isalnum.c), [`ft_isascii`](https://github.com/rumeysaispay/Libft/blob/main/ft_isascii.c), [`ft_isprint`](https://github.com/rumeysaispay/Libft/blob/main/ft_isprint.c)
Dönüştürme        | [`ft_toupper`](https://github.com/rumeysaispay/Libft/blob/main/ft_toupper.c), [`ft_tolower`](https://github.com/rumeysaispay/Libft/blob/main/ft_tolower.c), [`ft_atoi`](https://github.com/rumeysaispay/Libft/blob/main/ft_atoi.c)
String İşlemleri | [`ft_strlen`](https://github.com/rumeysaispay/Libft/blob/main/ft_strlen.c), [`ft_strchr`](https://github.com/rumeysaispay/Libft/blob/main/ft_strchr.c), [`ft_strrchr`](https://github.com/rumeysaispay/Libft/blob/main/ft_strrchr.c), [`ft_strncmp`](https://github.com/rumeysaispay/Libft/blob/main/ft_strncmp.c), [`ft_strlcpy`](https://github.com/rumeysaispay/Libft/blob/main/ft_strlcpy.c), [`ft_strlcat`](https://github.com/rumeysaispay/Libft/blob/main/ft_strlcat.c), [`ft_strdup`](https://github.com/rumeysaispay/Libft/blob/main/ft_strdup.c), [`ft_strnstr`](https://github.com/rumeysaispay/Libft/blob/main/ft_strnstr.c), [`ft_substr`](https://github.com/rumeysaispay/Libft/blob/main/ft_substr.c), [`ft_strjoin`](https://github.com/rumeysaispay/Libft/blob/main/ft_strjoin.c), [`ft_strtrim`](https://github.com/rumeysaispay/Libft/blob/main/ft_strtrim.c), [`ft_split`](https://github.com/rumeysaispay/Libft/blob/main/ft_split.c), [`ft_striteri`](https://github.com/rumeysaispay/Libft/blob/main/ft_striteri.c), [`ft_strmapi`](https://github.com/rumeysaispay/Libft/blob/main/ft_strmapi.c)
Bellek İşlemleri | [`ft_memset`](https://github.com/rumeysaispay/Libft/blob/main/ft_memset.c), [`ft_bzero`](https://github.com/rumeysaispay/Libft/blob/main/ft_bzero.c), [`ft_memcpy`](https://github.com/rumeysaispay/Libft/blob/main/ft_memcpy.c), [`ft_memmove`](https://github.com/rumeysaispay/Libft/blob/main/ft_memmove.c), [`ft_memchr`](https://github.com/rumeysaispay/Libft/blob/main/ft_memchr.c), [`ft_memcmp`](https://github.com/rumeysaispay/Libft/blob/main/ft_memcmp.c), [`ft_calloc`](https://github.com/rumeysaispay/Libft/blob/main/ft_calloc.c)
Yazdırma | [`ft_putchar_fd`](https://github.com/rumeysaispay/Libft/blob/main/ft_putchar_fd.c), [`ft_putstr_fd`](https://github.com/rumeysaispay/Libft/blob/main/ft_putstr_fd.c), [`ft_putendl_fd`](https://github.com/rumeysaispay/Libft/blob/main/ft_putendl_fd.c), [`ft_putnbr_fd`](https://github.com/rumeysaispay/Libft/blob/main/ft_putnbr_fd.c)
Yardımcı Fonksiyonlar | [`ft_itoa`](https://github.com/rumeysaispay/Libft/blob/main/ft_itoa.c)
Bağlı Liste (bonus) | ft_lstnew, ft_lstadd_front, ft_lstadd_back, ft_lstdelone, ft_lstclear, ft_lstiter, ft_lstmap, ft_lstsize, ft_lstlast

# ⚙️ Yapı Dosyaları
## 📄 Makefile
Bu dosya, projedeki tüm .c dosyalarının nasıl derleneceğini ve .a uzantılı statik bir kütüphane (libft.a) haline getirileceğini tanımlar.
make komutu ile çalıştırıldığında otomatik olarak tüm gerekli dosyalar derlenir.

Kullanımı:
```
bash
Kopyala
Düzenle
make        # Libft kütüphanesini derler
make clean  # Derleme sırasında oluşan .o dosyalarını siler
make fclean # .o dosyaları ve libft.a dosyasını siler
make re     # Yeniden derleme yapar (clean + make)
```
## 📄 libft.h
Bu dosya, projedeki tüm fonksiyon prototiplerini, gerekli kütüphane tanımlarını ve bağlı liste yapıları gibi struct tanımlarını içerir.
Tüm .c dosyaları bu dosyayı #include "libft.h" ile kullanır.

