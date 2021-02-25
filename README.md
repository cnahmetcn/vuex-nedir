# VueX

## Nedir? Neden Kullanıyoruz?
Vuex, uygulamalarımızda ki data yönetim paradigmasıdır. **State**, **Getters**,
**Mutations**, **Actions** ve **Modules** konseptleri vardır. 

Data yı yönetmek zor bir iştir. Data nın her zaman Single Source of Truth (SSOT) olması gerekmektedir. Yani en doğru ve güvenilir şekilde tutulması demektir. Bu sayede data belli bir sistemle ve yöntemle güncellenmeye başlıyor. (Unidirectional) tek yön olarak.

Uygulamamızdaki bütün component ler data ya istediği zaman ulaşabiliyor ve istediği zaman değiştirebiliyor. Bir yerde yazdığımız bir kodu başka bir yerde kullanıp değiştirmek istediğimizde **Actions** yada **Mutations** kullanarak data yı değiştirebiliyoruz. 

![alt text](https://vuex.vuejs.org/vuex.png)

- **`State`** proje içerisinde kullanacağımız veriler için oluşturduğumuz değişkenlerin bulunduğu bir javascript objesidir diyebiliriz. Bu state e göre Vue Components oluşturulur. Ne zaman state değişirse Vue Components de ona göre şekil alarak değişir. Örneğin bir buton koyduğumuzda Vue Components değişir. Ardından **Actions** dispatch edilir. **Actions**  kendi içerisinde bir **Mutations** commit ediyor. Bu **Mutations** da **State** i değiştiriyor. Döngü bu şekilde devam ediyor. 

![alt text](https://vuex.vuejs.org/flow.png)

## Vuex Konseptleri


## Vuex Olmadan Nasıl Yapabiliriz?

