# Ödev - Üniversite Yönetim Sistemi

 Üniversiteye ait sınıflıklar, çalışma ofisleri ve departmanlar vardır.

Departmanlara ait ofisler vardır.

Üniversiteye ait çalışanlar vardır. Bu çalışanlar profesör veya memur olabilir.

Her çalışan bir ofiste çalışır.

Bu sistemi tasvir eden Class (Sınıf) diyagramını çiziniz.

Not : Sınıflara ait nitelik ve davranışların belirtilmesine gerek yoktur.

[Link Yuml.me](https://yuml.me/diagram/scruffy/class/draw)

``` YUML
// Class Diagram
// -------------------

[Üniversite]<>1-1..*[Sınıflık]
[Üniversite]<>1-1..*[Çalışan]<>[Memur]<1-1..*>[Çalışma Ofisi]
[Üniversite]<>1-1..*[Çalışma Ofisi]<1-1..*>[Profesör]
[Üniversite]<>1-1..*[Departman]<>1-1..*[Çalışma Ofisi]

[Çalışan]<>[Profesör]
```

![UML Diagram](https://yuml.me/85d5e04a.png)